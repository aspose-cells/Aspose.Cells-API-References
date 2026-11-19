---
title: "LightCellsDataHandler"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le gestionnaire de données des cellules pour la lecture de gros fichiers de feuille de calcul en mode léger."
type: docs
url: /fr/java/com.aspose.cells/lightcellsdatahandler/
---
```
public interface LightCellsDataHandler
```

Représente le gestionnaire de données des cellules pour la lecture de gros fichiers de feuille de calcul en mode léger.

**Remarks**

Lors de la lecture d'un classeur avec ce mode, [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) sera appelée lors de la lecture de chaque feuille de calcul du classeur. Pour une feuille, si [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) renvoie true, alors toutes les données et propriétés des lignes/cellules de cette feuille seront vérifiées et traitées par l'implémentation de cette interface. Pour chaque ligne, [startRow(int)](../../com.aspose.cells/lightcellsdatahandler\#startRow-int-) sera appelée pour vérifier si elle doit être traitée. Si une ligne doit être traitée, les propriétés de cette ligne seront d'abord lues et l'utilisateur peut accéder à ses propriétés via [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-). Si les cellules de la ligne doivent également être traitées, alors [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-) doit renvoyer true et ensuite [startCell(int)](../../com.aspose.cells/lightcellsdatahandler\#startCell-int-) sera appelée pour chaque cellule existante de cette ligne afin de vérifier si une cellule doit être traitée. Si une cellule doit être traitée, alors [processCell(Cell)](../../com.aspose.cells/lightcellsdatahandler\#processCell-Cell-) sera appelée pour traiter la cellule par l'implémentation de cette interface.

Veuillez noter que l'utilisateur ne doit manipuler que les valeurs et les propriétés de l'objet Row/Cell actuel fourni par la méthode correspondante. Comme les données des cellules sont lues à partir du fichier modèle de manière flux, la plupart des autres objets peuvent être réinitialisés/mis à jour plus tard après le chargement des données des cellules. Ainsi, lorsque l'utilisateur manipule d'autres objets dans cette implémentation, ces opérations peuvent ne pas pouvoir affecter les objets existants dans le classeur. Ou pire encore, ces opérations peuvent entraîner des données incohérentes dans le classeur et provoquer ensuite un problème ou une exception inattendue. Donc, pour tous les autres objets tels que les formes, la largeur des colonnes et les styles, les mises en forme conditionnelles, ...etc., veuillez ne pas les manipuler dans les méthodes de cette implémentation. Au lieu de cela, veuillez les gérer après la construction du classeur.
## Méthodes

| Méthode | Description |
| --- | --- |
| [processCell(Cell cell)](#processCell-com.aspose.cells.Cell-) | Commence à traiter une cellule. |
| [processRow(Row row)](#processRow-com.aspose.cells.Row-) | Commence à traiter une ligne. |
| [startCell(int columnIndex)](#startCell-int-) | Prépare le traitement d'une cellule. |
| [startRow(int rowIndex)](#startRow-int-) | Prépare le traitement d'une ligne. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Commence à traiter une feuille de calcul. |
### processCell(Cell cell) {#processCell-com.aspose.cells.Cell-}
```
public abstract boolean processCell(Cell cell)
```


Commence à traiter une cellule.

**Remarks**

Elle sera appelée après la lecture des données d'une cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Objet Cell en cours de traitement |

**Returns:**
booléen - indique si cette cellule doit être conservée dans le modèle de cellules de la feuille actuelle. En général, il doit être false afin que toutes les cellules ne soient pas conservées en mémoire après leur traitement, ce qui permet d'économiser de la mémoire. Pour certains besoins spécifiques, comme lorsque l'utilisateur doit accéder à certaines cellules plus tard après le traitement complet du classeur, l'utilisateur peut faire en sorte que cette méthode renvoie true pour conserver ces cellules spéciales dans le modèle Cells et y accéder ultérieurement via des API telles que Cells[row, column]. Cependant, conserver les données des cellules dans le modèle Cells nécessite davantage de mémoire et, si toutes les cellules sont conservées, la lecture du fichier modèle en mode LightCells devient identique à la lecture en mode normal.
### processRow(Row row) {#processRow-com.aspose.cells.Row-}
```
public abstract boolean processRow(Row row)
```


Commence à traiter une ligne.

**Remarks**

Elle sera appelée après la lecture des propriétés de la ligne telles que la hauteur, le style, ...etc. Cependant, les cellules de cette ligne n'ont pas encore été lues.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Objet Row en cours de traitement. |

**Returns:**
booléen - indique si les cellules de cette ligne doivent être traitées. false pour ignorer toutes les cellules de cette ligne.
### startCell(int columnIndex) {#startCell-int-}
```
public abstract boolean startCell(int columnIndex)
```


Prépare le traitement d'une cellule.

**Remarks**

Il sera appelé lorsqu'une cellule existante de la ligne actuelle est atteinte. La ligne actuelle est la ligne du dernier appel de [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| columnIndex | int | indice de colonne de la cellule à traiter |

**Returns:**
booléen - indique si cette cellule doit être traitée. false pour ignorer la cellule et vérifier la suivante jusqu'à atteindre la fin des données de cellules de la ligne actuelle
### startRow(int rowIndex) {#startRow-int-}
```
public abstract boolean startRow(int rowIndex)
```


Prépare le traitement d'une ligne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | int | l'indice de la prochaine ligne à traiter |

**Returns:**
booléen - indique si cette ligne (propriétés ou données de cellules) doit être traitée. false pour ignorer cette ligne et ses cellules et vérifier la ligne suivante.
### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public abstract boolean startSheet(Worksheet sheet)
```


Commence à traiter une feuille de calcul.

**Remarks**

Il sera appelé avant la lecture des données de cellules d'une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | la feuille de calcul dont lire les données de cellules. |

**Returns:**
booléen - indique si les données de cellules de cette feuille doivent être traitées. false pour ignorer cette feuille.
