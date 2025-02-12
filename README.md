# Flatpak for Camunda Modeler
```
flatpak install flathub org.freedesktop.Sdk//24.08
flatpak install flathub org.electronjs.Electron2.BaseApp//24.08
flatpak-builder --user --install --force-clean build-dir com.camunda.Modeler.yaml
flatpak-builder --user --install --force-clean build-dir com.camunda.Modeler.Plugin.Linter.yaml
flatpak-builder --user --install --force-clean build-dir com.camunda.Modeler.Plugin.TransactionBoundaries.yaml
```
