# AddOn Veröffentlichung

- [Erstellung des AddOn-Keys](#anker-addon-key)
- [Mein API-Key](#anker-api-key)
- [Das Installer-AddOn](#anker-installer)
- [Veröffentlichen einer Version](#anker-addon-version)
  - [Settings](#anker-addon-version-settings)
  - [Meine Packages](#anker-addon-version-meinepackages)
  - [Eigenes AddOn](#anker-addon-version-eigenesaddon)
  - [AddOn-Version aktualisieren / löschen](#anker-addon-version-aktualisieren)
  - [AddOn-Version erstellen](#anker-addon-version-erstellen)


Um eigene AddOns zu veröffentlichen sollten man folgenden Weg nehmen.

<a name="anker-addon-key"></a>
## Erstellung des AddOn-Keys

Jedes AddOn hat einen eindeutige Kennung. Diese Kennung nennen wir Key. Diese Kennung ist gleichzeitig auch der Ordnername. Um einen passenden Key zu registrieren und auch die Bezeichung und Beschreibung des AddOns festzulegen, muss man sich zunächst in MyREDAXO [registrieren](/registrierung/) und dann [einloggen](/myredaxo/login/). Unter *Meine AddOns* kann dann die AddOn-Definition mit dem passenden Key angelegt werden. 

<a name="anker-api-key"></a>
## Mein API-Key

Um verschiedene weitere Aktionen durchführen zu können, die man nun auf der eigenen REDAXO Installation machen muss, braucht man einen API-Key. Diesen kann man sich in MyREDAXO erstellen. Dieser besteht aus einer Zeichenkette und sollte nicht weitergegeben werden, da man mit dem Key und dem eigenen Login Versionen veröffentlichen, löschen oder ändern kann.

<a name="anker-installer"></a>
## Das Installer-AddOn

Jede aktuelle REDAXO-Version hat einen Installer. Darüber werden AddOns installiert und aktualisiert, aber auch eigene AddOns  erstellt, bearbeitet und veröffentlicht.

<a name="anker-addon-version"></a>
## Veröffentlichen einer Version

<a name="anker-addon-version-settings"></a>
### Settings

Einzelne Versionen müssen entwickelt und geprüft werden. Das macht man meistens lokal auf dem eigenen Rechner. Hier muss das AddOn, welches man veröffentlichen will, existieren. Zunächst muss aber der API-Key in den Installer Einstellungen eingetragen werden. Nur dadurch kann erkannt werden, zu welchen AddOns man Zugriff hat. 

![Settings](/assets/v5.3.0-installer-settings.png)
Einstellungsdialog

<a name="anker-addon-version-meinepackages"></a>
### Meine Packages

Nun kann man über **Core & Packages/Eigene hochladen** einsehen, welche AddOns bereits registriert sind und auch in der lokalen Installation vorhanden sind. 
Das heißt, wenn mann Änderungen durchführen möchte und eine neue Version eines AddOns veröffentlichen möchte, muss genau dieses AddOn in der lokalen Installation zur Verfügung stehen. 

![Meine Packages](/assets/v5.3.0-installer-meinepackages.png)
Eigene hochladen - Meine Packeges

<a name="anker-addon-version-eigenesaddon"></a>
### Eigenes AddOn
Um ein ein Addon zu veröffentlichen oder eine neue Version aufzuspielen, wählt man das gewünschte AddOn in der Liste aus. 
In dieser Liste können einzelne Versionen mit "Datei aktualisieren" aktualisiert werden oder über das "+" eine neue Version erstellt werden. 


![Eigenes Addon](/assets/v5.3.0-installer-eigenesaddon.png)
Eigenes Addon

<a name="anker-addon-version-aktualisieren"></a>
### AddOn-Version aktualisieren / löschen

Eine Aktualisierung wird mit den vorhandenen Versionsinfos abgeglichen. D.h. wenn lokal eine spezielle Version läuft, dann kann man in den anderen Versionen nur die Beschreibung und den Status ändern. Sofern die ausgewählte Version mit der lokalen übereinstimmt, oder man auf "ZIP-Datei erstellen und hochlanden" klickt, kann man die eigene lokale Version komplett hochladen und ersetzen.

Eine einzelne Version kann man über den Löschen-Button aus dem Online-Archiv entfernen.

![Addon aktualisieren](/assets/v5.3.0-installer-addon-aktualisieren.png)
Addon aktualisieren

<a name="anker-addon-version-erstellen"></a>
### AddOn-Version erstellen

Versionen werden direkt aus dem lokalen AddOn selbst herangezogen (package.yml). Diese Version ist entsprechend voreingestellt und die Beschreibung und der Status können gesetzt werden. Sofern diese Version online gestellt wird, ist sie sofort für anderen REDAXO User verfügbar. Mit "Assets aus dem Root-Assets-Ordner nehmen" können Assets aus dem REDAXO Assets-Ordner übernommen werden.

![AddOn erstellen](/assets/v5.3.0-installer-addon-version-erstellen.png)
Addon erstellen