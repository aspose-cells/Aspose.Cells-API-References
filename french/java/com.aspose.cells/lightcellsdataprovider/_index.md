---
title: "LightCellsDataProvider"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le fournisseur de données pour l'enregistrement de gros fichiers de feuille de calcul en mode léger."
type: docs
url: /fr/java/com.aspose.cells/lightcellsdataprovider/
---
```
public interface LightCellsDataProvider
```

Représente le fournisseur de données pour l'enregistrement de gros fichiers de feuille de calcul en mode léger.

**Remarks**

Lors de l'enregistrement d'un classeur avec ce mode, [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-) sera vérifié lors de l'enregistrement de chaque feuille de calcul du classeur. Pour une feuille, si [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-) renvoie true, alors toutes les données et propriétés à enregistrer pour les lignes/cellules de cette feuille seront fournies par l'implémentation de cette interface. Tout d'abord, [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--) sera appelé pour obtenir l'index de la prochaine ligne à enregistrer. Si un index de ligne valide est retourné (l'index de ligne doit être en ordre croissant pour les lignes à enregistrer), alors un objet Row représentant cette ligne sera fourni par [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-) afin que l'implémentation définisse ses propriétés. Pour une ligne, [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--) sera d'abord vérifié. Si un index de colonne valide est retourné (l'index de colonne doit être en ordre croissant pour toutes les cellules de la ligne actuelle), alors un objet Cell représentant cette cellule sera fourni par [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\#startCell-Cell-) pour que l'implémentation définisse ses données et propriétés. Après [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\#startCell-Cell-) la cellule sera enregistrée directement dans le fichier de feuille de calcul résultant. Ensuite, la cellule suivante sera vérifiée et traitée.

Veuillez noter que l'utilisateur ne doit mettre à jour que les valeurs et les propriétés de l'objet Row/Cell actuel fourni par la méthode correspondante. Comme les données des cellules sont écrites dans le fichier résultant de manière flux, la plupart des autres objets peuvent déjà avoir été écrits dans le fichier résultant, ou avoir été rassemblés et écrit certaines données globales pour eux. Ainsi, lorsque l'utilisateur met à jour d'autres objets pendant la sauvegarde des données des cellules, ces opérations peuvent ne pas pouvoir affecter les données enregistrées. Ou pire encore, ces opérations peuvent entraîner l'enregistrement de données incohérentes dans le fichier résultant et finalement corrompre le fichier. Donc, pour tous les autres objets tels que les formes, la largeur des colonnes et les styles, les mises en forme conditionnelles, ...etc., veuillez ne pas les manipuler dans les méthodes de cette implémentation. Au lieu de cela, veuillez les gérer et les ajuster à l'état final avant d'appeler la méthode "Save" du classeur.
## Méthodes

| Méthode | Description |
| --- | --- |
| [isGatherString()](#isGatherString--) | Vérifie si la valeur de chaîne actuelle de la cellule doit être rassemblée dans un pool global. |
| [nextCell()](#nextCell--) | Obtient la cellule suivante à enregistrer. |
| [nextRow()](#nextRow--) | Obtient la ligne suivante à enregistrer. |
| [startCell(Cell cell)](#startCell-com.aspose.cells.Cell-) | Commence à enregistrer les données d'une cellule. |
| [startRow(Row row)](#startRow-com.aspose.cells.Row-) | Commence à enregistrer les données d'une ligne. |
| [startSheet(int sheetIndex)](#startSheet-int-) | Commence à enregistrer une feuille de calcul. |
### isGatherString() {#isGatherString--}
```
public abstract boolean isGatherString()
```


Vérifie si la valeur de chaîne actuelle de la cellule doit être rassemblée dans un pool global.

**Remarks**

La collecte des valeurs de chaîne ne sera avantageuse que lorsqu'il existe de nombreuses valeurs de chaîne dupliquées pour les cellules fournies par cette implémentation. Dans cette situation, la collecte des chaînes permet d'économiser beaucoup de mémoire et de générer un fichier résultant plus petit. Si de nombreuses valeurs de chaîne sont fournies par LightCellsDataProvider mais que peu d'entre elles sont identiques, la collecte des chaînes coûtera plus de mémoire et de temps et n'apportera aucun avantage au fichier résultant.

**Returns:**
booléen - vrai si la valeur de chaîne doit être rassemblée dans un pool global pour le fichier résultant.
### nextCell() {#nextCell--}
```
public abstract int nextCell()
```


Obtient la cellule suivante à enregistrer.

**Remarks**

Elle sera appelée au début de l'enregistrement d'une cellule.

**Returns:**
int - indice de colonne de la cellule suivante à enregistrer. -1 signifie que la fin des données de la ligne actuelle a été atteinte et qu'aucune autre cellule de la ligne actuelle ne doit être enregistrée.
### nextRow() {#nextRow--}
```
public abstract int nextRow()
```


Obtient la ligne suivante à enregistrer.

**Remarks**

Elle sera appelée au début de l'enregistrement d'une ligne et de ses données de cellules (avant [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\\#startRow-Row-)).

**Returns:**
int - l'indice de la prochaine ligne à enregistrer. -1 signifie que la fin des données de la feuille actuelle a été atteinte et qu'aucune autre ligne de la feuille actuelle ne doit être enregistrée.
### startCell(Cell cell) {#startCell-com.aspose.cells.Cell-}
```
public abstract void startCell(Cell cell)
```


Commence à enregistrer les données d'une cellule.

**Remarks**

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Objet Cell pour que l'implémentation remplisse les données. Son indice de colonne est la valeur renvoyée par le dernier appel de [nextCell()](../../com.aspose.cells/lightcellsdataprovider\\#nextCell--). Si la cellule a été initialisée dans le modèle interne des cellules, l'objet Cell existant sera utilisé. Sinon, un objet Cell temporaire sera utilisé pour que l'implémentation remplisse les données. |

### startRow(Row row) {#startRow-com.aspose.cells.Row-}
```
public abstract void startRow(Row row)
```


Commence à enregistrer les données d'une ligne.

**Remarks**

Elle sera appelée au début de l'enregistrement d'une ligne et de ses données de cellules. Si la ligne actuelle possède des propriétés personnalisées telles que la hauteur, le style, ...etc., l'implémentation doit définir ces propriétés sur l'objet Row fourni ici.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Objet Row pour que l'implémentation remplisse les données. Son indice de ligne est la valeur renvoyée par le dernier appel de [nextRow()](../../com.aspose.cells/lightcellsdataprovider\\#nextRow--). Si la ligne a été initialisée dans le modèle interne des cellules, l'objet Row existant sera utilisé. Sinon, un objet Row temporaire sera utilisé pour que l'implémentation remplisse les données. |

### startSheet(int sheetIndex) {#startSheet-int-}
```
public abstract boolean startSheet(int sheetIndex)
```


Commence à enregistrer une feuille de calcul.

**Remarks**

Elle sera appelée au début de l'enregistrement d'une feuille de calcul lors de l'enregistrement d'un classeur. Si le fournisseur doit se référer à *`sheetIndex`* plus tard dans la méthode startRow(Row) ou startCell(Cell), c'est-à-dire si le processus doit savoir quelle feuille de calcul est en cours de traitement, l'implémentation doit conserver la valeur *`sheetIndex`* ici.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | int | indice de la feuille actuelle à enregistrer. |

**Returns:**
booléen - vrai si ce fournisseur fournira les données pour la feuille donnée ; faux si la feuille donnée doit utiliser son modèle de données normal (Cells).
