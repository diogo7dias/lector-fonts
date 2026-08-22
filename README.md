# lector-fonts

Pre-built `.cpfont` SD card fonts for [lector](https://github.com/diogo7dias/lector) readers.

26 families, point sizes 10 to 18 (OpenDyslexic 8 to 16).

## Installing

- **On the device:** Settings > System > Manage Fonts, with Wi-Fi connected. The reader reads
  the `fonts.json` manifest from the release matching its own manifest and binary versions.
- **By hand:** download a family's files from the latest release and copy them into
  `/.fonts/<Family>/` on the SD card.

## Releases

Tags follow `sd-fonts-m<manifest version>-b<cpfont binary version>`. That tag is a moving
pointer to the current build; `-r<n>` suffixed tags are the immutable revisions behind it.

## Building

The fonts are generated from [`lib/EpdFont/scripts/sd-fonts.yaml`](https://github.com/diogo7dias/lector/blob/main/lib/EpdFont/scripts/sd-fonts.yaml)
in the firmware repository. This repository only carries the built artifacts.

## Licences

Every published family is redistributable: SIL Open Font License 1.1, except XCharter, which
uses the original Bitstream Charter free licence. Licence texts ship with the font sources in
the firmware repository.
