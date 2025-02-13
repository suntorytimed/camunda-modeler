# Unofficial Flatpak for Camunda Modeler
This repository provides an unofficial flatpak for [Camunda Modeler](https://github.com/camunda/camunda-modeler)
```
flatpak install flathub org.freedesktop.Sdk//24.08
flatpak install flathub org.electronjs.Electron2.BaseApp//24.08
flatpak-builder --user --install --force-clean build-dir io.github.suntorytimed.camunda-modeler.yaml
flatpak-builder --user --install --force-clean build-dir io.github.suntorytimed.camunda-modeler.Plugin.Linter.yaml
flatpak-builder --user --install --force-clean build-dir io.github.suntorytimed.camunda-modeler.Plugin.TransactionBoundaries.yaml
```
