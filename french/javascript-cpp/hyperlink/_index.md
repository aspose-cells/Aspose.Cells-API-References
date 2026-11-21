---
title: Hyperlink
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents a hyperlink.
type: docs
url: /fr/javascript-cpp/hyperlink/
---

## Hyperlink class

Encapsulates the object that represents a hyperlink.

```javascript
class Hyperlink;
```


### Example
```javascript
const { Workbook, SaveFormat } = AsposeCells;

//Instanciation d'un objet Workbook
var workbook = new Workbook();
//Ajout d'une nouvelle feuille de calcul à l'objet Workbook
workbook.worksheets.add();
//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
var worksheet = workbook.worksheets.get(0);
//Ajouter un lien hypertexte vers une URL dans la cellule "A1"
worksheet.hyperlinks.add("A1", 1, 1, "https://www.aspose.com");
//Enregistrement du fichier Excel
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [address](#address--)| string | Represents the address of a hyperlink. |
| [textToDisplay](#textToDisplay--)| string | Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink. |
| [area](#area--)| CellArea | Readonly. Gets the range of hyperlink. |
| [screenTip](#screenTip--)| string | Returns or sets the ScreenTip text for the specified hyperlink. |
| [linkType](#linkType--)| TargetModeType | Readonly. Gets the link type. |

## Methods

| Method | Description |
| --- | --- |
| [delete()](#delete--)| Deletes this hyperlink |


### address {#address--}

Represents the address of a hyperlink.

```javascript
address : string;
```


### textToDisplay {#textToDisplay--}

Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink.

```javascript
textToDisplay : string;
```


### area {#area--}

Readonly. Gets the range of hyperlink.

```javascript
area : CellArea;
```


### screenTip {#screenTip--}

Returns or sets the ScreenTip text for the specified hyperlink.

```javascript
screenTip : string;
```


### linkType {#linkType--}

Readonly. Gets the link type.

```javascript
linkType : TargetModeType;
```


### delete() {#delete--}

Deletes this hyperlink

```javascript
delete() : void;
```



