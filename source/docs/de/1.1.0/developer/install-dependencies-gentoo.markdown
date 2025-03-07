---
Type:            article
Title:           Abhängigkeiten für Gentoo installieren
Project:         HandBrake
Project_URL:     https://handbrake.fr/
Project_Version: 1.1.0
Language:        English
Language_Code:   en
Authors:         [ Bernhard Rader (raderb), Bradley Sepos <bradley@bradleysepos.com> (BradleyS) ]
Copyright:       2024 HandBrake Team
License:         Creative Commons Attribution-ShareAlike 4.0 International
License_Abbr:    CC BY-SA 4.0
License_URL:     https://handbrake.fr/docs/license.html
---

Abhängigkeiten für Gentoo installieren
=================================

Die folgenden Anweisungen sind für [Gentoo](https://gentoo.org) Profil `default/linux/amd64/17.0` mit Portage snapshot 20180520 (nur HandBrake [CLI](abbr:Command Line Interface - Kommandozeile)).

Grundvoraussetzungen um Kommandos zu starten:

- sudo (für standard user accounts)

Abhängigkeiten[^rebuild]:

- fribidi
- dev-vcs/git
- harfbuzz
- jansson
- lame
- libass
- libogg
- libsamplerate
- libtheora
- libvorbis
- opus
- x264

Abhängigkeiten installieren:

    sudo emerge --ask fribidi dev-vcs/git harfbuzz jansson lame libass libogg libsamplerate libtheora libvorbis opus x264

Gentoo ist nun bereit HandBrake zu bauen. Siehe [HandBrake für Linux bauen](build-linux.html) für mehr Anweisungen.

[^rebuild]: Zuvor installierte Abhängigkeiten müssen eventuell vor dem HandBrake Build neu gebaut werden.
