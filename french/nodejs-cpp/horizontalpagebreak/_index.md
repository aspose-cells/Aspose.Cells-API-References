---
title: HorizontalPageBreak
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents a horizontal page break.
type: docs
url: /fr/nodejs-cpp/horizontalpagebreak/
---

## HorizontalPageBreak class

Encapsulates the object that represents a horizontal page break.

```javascript
class HorizontalPageBreak;
```


### Example
```javascript
const { Workbook } = require("aspose.cells.node");

//Instanciation d'un objet Workbook
var workbook = new Workbook();

//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
var worksheet = workbook.worksheets.get(0);

//Ajouter un saut de page à la cellule Y30
var Index = worksheet.horizontalPageBreaks.add("Y30");

//obtenir le saut de page horizontal nouvellement ajouté
var hPageBreak = worksheet.horizontalPageBreaks.get(Index);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [startColumn](#startColumn--)| number | Readonly. Gets the start column index of this horizontal page break. |
| [endColumn](#endColumn--)| number | Readonly. Gets the end column index of this horizontal page break. |
| [row](#row--)| number | Readonly. Gets the zero based row index. |

## Methods

| Method | Description |
| --- | --- |
| [getStartColumn()](#getStartColumn--)| <b>@deprecated.</b> Please use the 'startColumn' property instead. Gets the start column index of this horizontal page break. |
| [getEndColumn()](#getEndColumn--)| <b>@deprecated.</b> Please use the 'endColumn' property instead. Gets the end column index of this horizontal page break. |
| [getRow()](#getRow--)| <b>@deprecated.</b> Please use the 'row' property instead. Gets the zero based row index. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### startColumn {#startColumn--}

Readonly. Gets the start column index of this horizontal page break.

```javascript
startColumn : number;
```


### endColumn {#endColumn--}

Readonly. Gets the end column index of this horizontal page break.

```javascript
endColumn : number;
```


### row {#row--}

Readonly. Gets the zero based row index.

```javascript
row : number;
```


### getStartColumn() {#getStartColumn--}

<b>@deprecated.</b> Please use the 'startColumn' property instead. Gets the start column index of this horizontal page break.

```javascript
getStartColumn() : number;
```


### getEndColumn() {#getEndColumn--}

<b>@deprecated.</b> Please use the 'endColumn' property instead. Gets the end column index of this horizontal page break.

```javascript
getEndColumn() : number;
```


### getRow() {#getRow--}

<b>@deprecated.</b> Please use the 'row' property instead. Gets the zero based row index.

```javascript
getRow() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



