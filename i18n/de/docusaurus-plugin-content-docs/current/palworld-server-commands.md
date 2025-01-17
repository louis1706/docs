---
id: palworld-server-commands
title: Palworld Server-Befehle
description: Informationen über nützliche Befehle für das Palworld-Spiel von ZAP-Hosting - ZAP-Hosting.com Dokumentation
sidebar_label: Server-Befehle
---

Palworld-Server verfügen über eine Reihe von nützlichen integrierten Serverbefehlen, die du im Spiel und über deine Serverkonsole verwenden kannst. In diesem Leitfaden werden wir uns mit vielen dieser Befehle befassen und Beschreibungen und Anwendungsbeispiele für jeden einzelnen geben.

<iframe width="560" height="315" src="https://www.youtube.com/embed/SDZC4-FEdNM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Admin einrichten

Du musst zuerst ein Admin-Passwort für deinen Palword-Server festlegen und dich selbst als Admin im Spiel hinzufügen, bevor du auf die Admin-Server-Befehle im nächsten Abschnitt zugreifen kannst.

Du kannst das Admin-Passwort deines Servers über den Reiter **Einstellungen** im Webinterface deines Servers oder über die Konfigurationsdatei **PalWorldSettings.ini** festlegen. Sobald du es festgelegt hast, kannst du den Befehl `AdminPasswort [Passwort]` im Spiel verwenden, um dich als Admin hinzuzufügen.

:::tip
Wir empfehlen dir, einen Blick in unseren [Palworld Setup Admin guide](palworld-admin.md) zu werfen, der ein spezieller Leitfaden für dieses Thema ist und genauere Informationen über das Festlegen eines Admin-Passworts und das Hinzufügen von Benutzern als Admin enthält.
:::

## Verfügbare Befehle

Die folgende Tabelle enthält eine Reihe von Serverbefehlen für Palworld sowie Beispiele und Beschreibungen, die im Spiel und über die Serverkonsole verwendet werden können.

Wenn der Parameter `steamid` benötigt wird, kannst du die SteamID eines Spielers einfach kopieren, indem du zweimal mit der rechten Maustaste auf die Spielerliste klickst.

:::info
Bevor du diese Befehle verwenden kannst, musst du ein Admin-Passwort einrichten und dir mit dem Befehl `/AdminPasswort` die entsprechenden Rechte erteilen. Andernfalls erhältst du eine Fehlermeldung. Lies den nächsten Abschnitt in diesem Leitfaden, um zu verstehen, wie du das machst.
:::

| Befehlssyntax               | Akzeptierte Werte | Beschreibung                                                                        | 
| --------------------------- | ----------------- | ----------------------------------------------------------------------------------- | 
| /Shutdown [secs] [message]  | Integer, String   | Schaltet den Server nach den angegebenen Sekunden ab, mit der dazugehörigen Meldung | 
| /DoExit                     | -                 | Erzwingt das Beenden des Servers                                                    | 
| /Broadcast                  | String            | Sende eine Nachricht an alle Spieler, die sich gerade auf dem Server befinden       | 
| /KickPlayer [steamid]       | String            | Kick den Zielspieler vom Server                                                     | 
| /BanPlayer [steamid]        | String            | Verbannt den Zielspieler vom Server                                                 | 
| /TeleportToPlayer [steamid] | String            | Teleport zum Zielspieler                                                            | 
| /TeleportToMe [steamid]     | String            | Teleportiere den Zielspieler zu dir                                                 | 
| /ShowPlayers                | -                 | Informationen über alle aktuell verbundenen Spieler bereitstellen                   | 
| /Info                       | -                 | Serverinformationen bereitstellen                                                   | 
| /Save                       | -                 | Die aktuellen Weltdaten speichern                                                   |

:::note
Du kannst eine Person derzeit nicht im Spiel sperren, da es keinen entsprechenden Befehl gibt. Du musst die Datei `banlist.txt` in deinem Server-Verzeichnis manuell bearbeiten, wenn du einen Spieler wieder sperren willst.
:::