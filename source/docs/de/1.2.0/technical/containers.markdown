---
Type:            article
State:           [ obsolete ]
Title:           Formate / Container
Project:         HandBrake
Project_URL:     https://handbrake.fr/
Project_Version: 1.2.0
Language:        Deutsch
Language_Code:   de
Authors:         [ Bernhard Rader (raderb), Scott (s55) ]
Copyright:       2024 HandBrake Team
License:         Creative Commons Attribution-ShareAlike 4.0 International
License_Abbr:    CC BY-SA 4.0
License_URL:     https://handbrake.fr/docs/license.html
---

Formate / Container
=============================
Container sind Dateien die Audio und Videospuren beinhalten. Sie verwalten die Spuren für das Abspielen und stellen zusätzliche Features bereit wie zum Beispiel Kapitelmarkierungen.

HandBrake unterstützt zwei weit verbreitete Formate: MKV und MP4 (auch als M4V bekannt).

## Features
Features und Kompatibilität variiert zwischen MKV und MP4. Es folgt eine Zusammenfassung von ein paar Unterschieden:

- In einer MP4 Datei kannst du MPEG-4 Video welches von ffmpeg oder x264 erstellt wurde abspeichern.
  - Es unterstützt H.264, H.265, MPEG-4 und MPEG-2 Video.
  - Es speichert Audio in dem AAC Format. Es ist außerdem mögich, Dolby Digital 5.1 Surround Sound (AC3) aus einer DVD in eine MP4 Datei durchzuleiten. Dies ist jedoch ein neuer Standard und wird noch nicht überall unterstützt. VLC kann es dekodieren und AppleTV kann es zu einem Surround Sound Receiver durchleiten.
  - MP4 unterstützt zudem Kapitel für welche HandBrake das Kapitelformat von Apple verwendet.
  - MP4 kann zudem Video mit variable Framerate (VFR) abspeichern.
  - Beachte, dass Kapitel und AC3 Audio in QuickTime nur sichtbar sind, wenn du die Dateiendung von .mp4 auf .m4v änderst. HandBrake macht dies für dich automatisch wenn du diese Features verwendest. Dies kann jedoch in den Einstellungen deaktiviert werden, wenn du unbedingt .mp4 als Dateiendung verwenden möchtest.
  - Das MP4 Format kann für einen "fast start" optimiert werden. Dies ist beim streamen bzw. für progressive downloads hilfreich.
  - Es kann außerdem "Soft" Untertitel inkludieren welche ein- und ausgeschalten werden können, anstatt immer in das Video hineingebrennt zu sein.

- In einer MKV Datei kannst du MPEG-4 Video welches von ffmpeg, x264 oder Theora erstellt wurde abspeichern.
  - Es unterstützt H.264, H.265, MPEG-4, MPEG-2 und VP3 (Vorbis)
  - Es speichert Audio in den Formaten AAC, MP3, Vorbis oder FLAC. Zusätzlich können die Formate Dolby Digital 5.1 (AC3) und Digital Theater Systems (DTS) durchgeleitet werden.
  - Das Format unterstützt Kapitel und variable Framerate (VFR) Video.
  - MKV kann gleich wie MP4 "soft" Untertitel verwenden welche ein- und ausgeschalten werden können, anstatt immer in das Video eingebrennt zu sein. Diese können entweder Bitmap Bilder oder Text sein.

## MP4 vs M4v

Diese beiden sind die exakt selben Dateien, der einzige Unterschied liegt in der Dateiendung - MP4 vs M4V.

Bei MP4 Dateien verwendet HandBrake automatisch die M4V Dateiendung wenn du AC3 Audio durchleitest, SRT Untertitel verwendest oder Kapitelmarkierungen aktiviert hast.

Du kannst die Dateiendung zwischen .mp4 und .m4v beliebig wechseln da die Datei unverändert bleibt. Es gibt keine Unterschiede in dem Inhalt oder dem Containerformat.

Due kannst die Option dafür in den Einstellungen aktivieren bzw. deaktivieren.

Beachte: QuickTime oder jegliche auf QT basierende Applikation kann eine MP4 Datei nicht abspielen wenn diese Features aktiviert sein, es sei denn es verfügt über die Dateiendung ".m4v".
