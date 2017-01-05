# Cours de sass (2016-2017)

## Description

Ce repo contient le code écrit durant le cours de sass à Pop School Lens, session 2016-2017.

## Utiliser sass

### obtenir de l'aide

    sass --help

### compiler un fichier sass en un fichier css

    sass style.sass style.css

### compiler un fichier scss en un fichier css

    sass style.scss style.css

#### traquer les changements dans le dossier sass/
#### et compiler dans le dossier css/

    sass --watch sass:css

#### compiler les fichiers sass dans différents styles

    # compiler automatiquement du code css dans un style « écrit à la main » (bon pour la version de dev)
    sass --watch -t expanded sass:css

    # compiler automatiquement du code css compressé (bon pour la version prod)
    sass --watch -t compressed sass:css

    # forcer la recompilation en style code « écrit à la main »
    sass --update -f -t expanded sass:css

    # forcer la recompilation en style code compressé
    sass --update -f -t compressed sass:css

## Convertir des fichier css, scss et sass en scss ou sass

### obtenir de l'aide

    sass-convert --help

### convertir un fichier css en fichier sass

    sass-convert --from css --to sass style.css style.sass

### convertir un fichier css en fichier scss

    sass-convert --from css --to scss style.css style.scss

### convertir un fichier scss en fichier sass

    sass-convert --from scss --to sass style.scss style.sass

### convertir un fichier sass en fichier scss

    sass-convert --from sass --to scss style.sass style.scss

### convertir tous les fichiers css d'un dossier en fichiers sass dans le dossier sass

    sass-convert -r --from css --to sass css sass

### convertir tous les fichiers css d'un dossier en fichiers scss dans le dossier sass

    sass-convert -r --from css --to scss css sass

