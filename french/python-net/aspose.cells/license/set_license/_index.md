---
title: set_license méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells/license/set_license/
is_root: false
---
##  set_license(license_name) {#str}
Licence du composant.



```python
def set_license(self, license_name):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| license_name | str |  |
###  Remarques

Essaie de trouver la licence aux emplacements suivants :


1. Chemin explicite.


2. Le dossier contenant l'assemblage de composants Aspose.


3. Le dossier qui contient l'assembly appelant du client.


4. Le dossier qui contient l'assembly d'entrée (démarrage).


5. Une ressource intégrée dans l'assembly appelant du client.


**Note:** Sur le Compact Framework .NET, essaie de trouver la licence uniquement dans ces emplacements :


1. Chemin explicite.


2. Une ressource intégrée dans l'assembly appelant du client.
###  Exemple


Dans cet exemple, une tentative sera faite pour trouver un fichier de licence nommé MyLicense.lic
 dans le dossier qui contient


le composant, dans le dossier qui contient l'assembly appelant,
dans le dossier de l'assembly d'entrée puis dans les ressources embarquées de l'assembly appelant.

```python
from aspose.cells import License

license = License()
license.set_license("MyLicense.lic")

```
Peut être un nom de fichier complet ou court ou le nom d'une ressource intégrée.
Utilisez une chaîne vide pour passer en mode d'évaluation.


##  set_license(stream) {#io.RawIOBase}
Licence du composant.



```python
def set_license(self, stream):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| stream | io.RawIOBase | Un flux qui contient la licence.|
###  Remarques

Utilisez cette méthode pour charger une licence à partir d'un flux.
###  Exemple


```python
from aspose.cells import License

license = License()
license.set_license(myStream)

```



###  Voir également
* module [aspose.cells](../../)
* classe [License](/cells/fr/python-net/aspose.cells/license)
