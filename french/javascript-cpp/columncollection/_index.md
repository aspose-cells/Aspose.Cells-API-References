---
title: ColumnCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Collection of the Column..column objects that represent the individual columnsettings in a worksheet. The Column object only represents the settings such as column width styles .etc. for the whole column has nothing to do with the fact that there are nonempty cellsdata or not in corresponding column. And the Count of this collection only represents the count Column objects that have been instantiated in this collection has nothing to do with the fact that there are nonempty cellsdata or not in the worksheet.
type: docs
url: /fr/javascript-cpp/columncollection/
---

## ColumnCollection class

Collection of the [Column](../column/) objects that represent the individual column(setting)s in a worksheet. The Column object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet.

```javascript
class ColumnCollection;
```


### Example
```javascript
const { Workbook, Color, BackgroundType, StyleFlag, SaveFormat } = AsposeCells;

//Instanciation d'un objet Workbook
var workbook = new Workbook();
//Obtenir la référence de la première feuille de calcul
var worksheet = workbook.worksheets.get(0);
//Ajouter un nouveau style au classeur
var style = workbook.createStyle();
//Définir la couleur d'arrière-plan en bleu
style.foregroundColor = Color.Blue;
//définir le motif d'arrière-plan
style.pattern = BackgroundType.Solid;
//Nouveau drapeau de style
var styleFlag = new StyleFlag();
//Définir tous les styles
styleFlag.all = true;

//Modifier la largeur par défaut des dix premières colonnes
for (var i = 0; i < 10; i++) {
    worksheet.cells.columns.get(i).width = 20;
}

//Obtenir la colonne avec un formatage non par défaut
var columns = worksheet.cells.columns;
var count = columns.count;
for (var i = 0; i < count; i++) {
    var column = columns.getColumnByIndex(i);
    //Appliquer le style aux dix premières colonnes
    column.applyStyle(style, styleFlag);
}

//Enregistrement du fichier Excel
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [Column](../column/) object by column index. The Column object of given column index will be instantiated if it does not exist before. |
| [getColumnByIndex(number)](#getColumnByIndex-number-)| Gets the [Column](../column/) object by the position in the list. |


### get(number) {#get-number-}

Gets a [Column](../column/) object by column index. The Column object of given column index will be instantiated if it does not exist before.

```javascript
get(columnIndex: number) : Column;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number |  |

**Returns**

[Column](../column/)

### getColumnByIndex(number) {#getColumnByIndex-number-}

Gets the [Column](../column/) object by the position in the list.

```javascript
getColumnByIndex(index: number) : Column;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The position in the list. |

**Returns**

Returns the column object.


