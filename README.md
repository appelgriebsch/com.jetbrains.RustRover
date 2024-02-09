# Introductions

## Checkout the sources incl. submodules

```
$ git submodule update --init
```

## Install flatpak dependencies 



## Build flatpak package

```
$ flatpak-builder .build com.jetbrains.RustRover.yml
```

## Create local repo

```
$ flatpak-builder --repo=../repo --force-clean .build com.jetbrains.RustRover.yml
```

## Install for current user

```
$ flatpak --user remote-add --no-gpg-verify local-test-repo ../repo
$ flatpak --user install local-test-repo com.jetbrains.RustRover
```
