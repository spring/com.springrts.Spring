# spring flatpak package

Flatpak package for spring
See https://springrts.com/

Buildbot info is available here https://flathub.org/builds/#/apps/com.springrts.Spring
A guide on flathub app maintenance is here: https://github.com/flathub/flathub/wiki/App-Maintenance

## Testing

Additional steps might be required to get flatpak working see 
https://docs.flatpak.org/en/latest/first-build.html

Build 

```
flatpak-builder --force-clean build-dir com.springrts.Spring.yaml
```

Test

```
flatpak-builder --run build-dir com.springrts.Spring.yaml spring
```

Install

```
flatpak-builder --install --user --force-clean build-dir com.springrts.Spring.yaml
```

Run installed version:
```
flatpak run com.springrts.Spring
```
