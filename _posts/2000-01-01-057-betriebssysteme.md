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

- Viele Android-Geräte werden vom Hersteller nur über einen kurzen Zeitraum mit Sicherheits-Updates versorgt. Dadurch sind die Geräte anfällig gegen viele Arten von Angriffen, z.B. durch Schadsoftware, die ungeschlossene Sicherheitslücken auf den Gerät nutzt.   
 - Praktisch alle Android-Smartphones kommen ab Werk mit den Google-Diensten. Diese sind tief ins System integriert und es ist praktisch unmöglich Datenabflüsse zu Google zu verhindern. Google hingegen ist mit der Kooperation mit den Repressionsbehörden verpflichtet.

#### Argumente gegen einen Betriebsystem-Wechsel

Durch [Verified Boot](https://source.android.com/security/verifiedboot) stellen Smartphones sicher, dass nur das unveränderte Betriebsystem des Herstellers gestartet werden kann. Dies schützt vor Schadsoftware, welche sich in das System verändern möchte und stellt eine Hürde für das Auslesen der Daten im Falle einer Beschlagnahme oder bei Verlust dar. Für die Installation vieler CustomROMs muss dieser Schutz allerdings deaktiviert werden. Dies stellt ein großes Sicherheitsproblem dar.

#### CustomROM Übersicht

__LineageOS__

Das wohl bekannteste alternative Betriebsystem für Android-Geräte ist [LineageOS](https://lineageos.org/). Es ist für sehr viele Geräte verfügbar und kommt ohne Google-Services, die nachträgliche Installation ist aber möglich. Dieses OS ist gerade für Geräte, die schon lange keine OS-Updates mehr bekommen eine gute Möglichkeit die Sicherheit gegen Schadsoftware zu erhöhen, bietet aber nicht die Möglichleit 'Verified Boot' zu nutzen. Wir raten daher aus dem oben genannten Grund eher davon ab.

__GrapheneOS__

Falls ihr ein Google Pixel euer eigenen nennt könnt ihr [GrapheneOS](https://grapheneos.org) nutzen. 




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

