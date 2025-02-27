# Unofficial Flatpak for Camunda Modeler
This repository provides an unofficial flatpak for [Camunda Modeler](https://github.com/camunda/camunda-modeler). This flatpak repackages the official release by the Camunda community project.

## Install runtime dependency
```
flatpak install -u org.freedesktop.Platform/x86_64/24.08
```
## Install from flatpak.hibiki.eu
Directly via flatpakref:
```
flatpak install -u https://flatpak.hibiki.eu/repo/appstream/io.github.suntorytimed.camunda-modeler.flatpakref
```
or by adding the repository including the GPG key:
```
flatpak remote-add -u --gpg-import=https://flatpak.hibiki.eu/repo/hibiki.pgp hibikiEU https://flatpak.hibiki.eu/repo/hibiki.flatpakrepo
flatpak install -u app/io.github.suntorytimed.camunda-modeler/x86_64/stable
# this would work as well: flatpak install -u camunda
```
You can also just download the [GPG key](https://flatpak.hibiki.eu/repo/hibiki.pgp) and [flatpakrepo file](https://flatpak.hibiki.eu/repo/hibiki.flatpakrepo) and add those via your GUI tool of choice (e.g. seahorse and GNOME Software). The GPG key is available on public keyservers as well:
* https://keys.openpgp.org/vks/v1/by-fingerprint/7DA1BE30D07020497D5F11EBDFEB41A553E3BD55

## Build it yourself
```
flatpak install flathub org.freedesktop.Sdk//24.08
flatpak install flathub org.electronjs.Electron2.BaseApp//24.08
flatpak-builder --user --install --force-clean build-dir io.github.suntorytimed.camunda-modeler.yaml
```
