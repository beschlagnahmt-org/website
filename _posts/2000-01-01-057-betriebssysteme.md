---
title: Betriebssysteme
layout: capter
permalink: /betriebssysteme/
category: capter
---
# Betriebssysteme
{:.no_toc}

<details markdown="block">
  <summary>
    Inhalt
  </summary>
* TOC
{:toc}
</details>

In diesem Kapitel geben wir die einen Überblick über die Betriebssysteme, die du auf deinen Geräten nutzen kannst. Es geht dabei um eine grundsätzliche Empfehlung, detailierte Tipps findest du in den anderen Kapiteln.

## Grundsätzliches zu Sicherheit

Nutze nur Geräte und Betriebsysteme, die noch mit Sicherheitsupdates versorgt werden. In Netz findest Du Informationen darüber wie lange Dein [Windows](https://support.microsoft.com/de-de/help/13853/windows-lifecycle-fact-sheet), Linux, [MacOS](https://www.apple.com/de/macos/how-to-upgrade/) oder [iOS](https://de.wikipedia.org/wiki/Versionsgeschichte_von_iOS#Aktuelle_Versionen) Sicherheitsupdates erhält. Bei Android-Smartphones ist es oft schwierig eine Aussage zu bekommen, ihr solltet aber kein Gerät benutzen, dessen [Sicherheitspatch-Level älter](https://www.tutonaut.de/android-version-und-sicherheitspatch-level-herausfinden/) als 6 Monate ist.

## Smartphone

An der Stelle nochmal der Hinweis: Bei Aktionen sollte das Smartphone in jedem Fall zuhause gelassen werden, falls ihr kein Aktionshandy braucht und zusätzlich genau wisst was ihr tut.

### Android

#### Argumente für einen Betriebsystem-Wechsel

- Viele Android-Geräte werden vom Herstekker nur über einen kurzen Zeitraum mit Sicherheits-Updates versorgt. Dadurch sind die Geräte anfällig gegen viele Arten von Angriffen, z.B. durch Apps, die ungeschlossene Sicherheitslücken auf den Gerät nutzen.   
 - Praktisch alle Android-Smartphones kommen ab Werk mit den Google-Diensten. Diese sind tief ins System integriert und es ist praktisch unmöglich Datenabflüsse zu Google zu verhindern. Google hingegen ist mit der Kooperation mit den Repressionsbehörden verpflichtet.
 - 

#### Argumente gegen einen Betriebsystem-Wechsel

https://source.android.com/security/verifiedboot



Damit ihr überhaupt soweit kommt, über die Wahl eures zukünftigen Betriebssystems zu philosophieren, müsst ihr in jedem Fall den Bootloader öffnen. Da liegt aber schon das erste Problem: 
Die überwiegende Mehrheit der alternativen Betriebssysteme belassen es einfach dabei und sperren den Bootloader im Anschluss der Installation nicht wieder. Dies bietet Angreifer:innen die Möglichkeit, eigene Software ins System zu schleusen und so eure Daten abzugreifen.
Ein weiteres Problem mit CustomROMS ist die Sorglosigkeit um Umgang mit ihnen. Die überwiegende Mehrheit möchte es vermutlich ausreizen, jetzt die volle Kontrolle über ihr Smartphone zu haben und installieren parallel auch gleich Software wie Magisk, die Anwendungen den Root-Zugriff auf euer Gerät ermöglichen.
Aber auch das bietet wieder einen enormen Angriffsvektor für Schadsoftware, der nun alle Möglichkeiten eures Gerätes zur Verfügung stehen, sollte diese Root-Zugriff erlangen. Und wenn wir schon beim unbedarften installieren von Software sind: GoogleApps ist da ebenfalls so ein Kandidat, der oft unnötigerweise mitinstalliert wird.
Es ist grundsätzlich davon abzuraten Konzerne tief in euer Smartphone zu lassen, die zweifelsohne mit den Repressionsbehörden kooperieren.

##### Bei welchen Betriebssystemen ihr diese Probleme nicht habt

Es gibt auch Betriebssysteme, da eine echte Alternative darstellen und den Datenschutz eures Geräts tatsächlich kompromisslos erhöhen. Uns sind während unserer Recherche da allerdings nur 2 Kandidaten aufgefallen: GrapheneOS & CalyxOS.
Beide Betriebssysteme bestehen darauf, dass im Anschluss der Installation der Bootloader wieder verschlossen wird. Somit ist sichergestellt, dass nur vom Betriebssystem zur Verfügung gestellte Updates installiert werden können. Diese funktionieren durch den integriegten Updater unkompliziert.
Zudem erlauben sie keinen Root-Zugriff und GoogleApps lassen sich ebenfalls nicht installieren (obwohl CalyxOS eine Kompromisslösung anbietet, dazu später mehr).
GrapheneOS verhält sich in der Verwendung nicht anders als ein gewöhnliches Android Telefon, kommt aber unter der Haube mit einigen teils sehr technischen Sicherheitsvorkehrungen. Um einige davon kurz zu benennen: 
- Standardmäßige Geräteverschlüsselung
- Sicherere & zufällige Speicherzuweisung
- Zufällige Zuweisung der normalerweise eindeutigen Geräteadresse (MAC-Randomisierung)
- Schutz vor stillen SMS - im Flugzeugmodus werden verantwortliche Module abgeschaltet
- remote attestation (regelmäßige Überprüfung der Integrität des Betriebssystems)
Weitere Infos gibt es hier: https://grapheneos.org/faq

Was es zu beachten gibt:
Durch die fehlenden Google Dienste funktionieren einige Apps nicht oder nur eingeschränkt. Einige Sicherheitsfeatures verlangsamen das Smartphone unwesentlich, was allerdings absolut zu verkraften ist. 
Das Betriebssystem ist aktuell nur für auf Google Pixel Smartphones verfügbar. Diese sind technisch betrachtet am besten geeignet für die vorgenommen Verbesserungen. Sollte das Projekt wachsen ist auch die Unterstützung für andere Geräte möglich, dies liegt allerdings nicht im Fokus.

Das meiste von dem bereits gesagtem gilt auch für CalyxOS, wobei die Sicherheitsfunktionen hier minimal weniger drastisch ausfallen und daher das System etwas flotter läuft. Mehr Infos findet ihr auf https://calyxos.org/ . 
Außerdem erlaubt CalyxOS die Installation von microG, eine Open Source Schnittstelle für GoogleApps, die die Verwendung einiger Google Services ermöglicht.
In unseren Augen ist microG leider ein unnötiger Kompromiss: Es funktionieren bei weitem nicht alle GoogleApps und dennoch bekommt google hierdurch wieder eingeschränkten Zugriff auf unser System. Wenn also wie bei uns Privatssphäre und Sicherheit kompromisslos im Vordergrund stehen, ist davo abzuraten.
Falls ihr es doch verwenden wollt, können wir euch https://plexus.techlore.tech/ ans Herz legen. Die Website verrät euch, welche Apps auch ohne GoogleApps bzw. mit microG funktionieren bzw. welche Einschränkungen es gibt.

### iOS

Das Phänomen "CustomROMS" spielt für iOS-Geräte keine Rolle. Seht auch davon ab bei euerem Gerät einen sogenannten 'Jailbreak' durch zu führen, da dies die Gerätsicherheit deutlich absenkt.

## Laptop / PC

### Windows



### Linux

Grundsätzlich vertrauenswürdiger. Verschlüsselung. Hardware vorher prüfen.

### MacOS

