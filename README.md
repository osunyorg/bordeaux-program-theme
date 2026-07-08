# Formation IUT Bordeaux - options de thème

## Utilisation

1. Importer le thème dans le site.

```bash
git submodule add git@github.com:osunyorg/bordeaux-program-theme.git themes/bordeaux-program-theme
```

2. Ajouter le plugin comme un thème dans `config/_default/config.yaml`. Ajouter également les logos.

```yaml
theme: bordeaux-program-theme
_merge: deep
params:
  logo:
    header: /assets/images/logo.svg
    footer: /assets/images/logo-white.svg
```

3. Appel des styles et options dans `assets/sass/main.sass`

```sass
@import "_configuration"
@import "bordeaux-program-theme/theme"
@import "bordeaux-program-theme/options/classic"
```

## Site 

- https://mp.iut.u-bordeaux.fr/
