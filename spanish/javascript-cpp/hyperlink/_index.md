---
title: Hyperlink
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents a hyperlink.
type: docs
url: /es/javascript-cpp/hyperlink/
---

## Hyperlink class

Encapsulates the object that represents a hyperlink.

```javascript
class Hyperlink;
```


### Example
```javascript
const { Workbook, SaveFormat } = AsposeCells;

//Instanciando un objeto Workbook
var workbook = new Workbook();
//Agregando una nueva hoja de trabajo al objeto Workbook
workbook.worksheets.add();
//Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
var worksheet = workbook.worksheets.get(0);
//Agregar un hipervínculo a una URL en la celda "A1"
worksheet.hyperlinks.add("A1", 1, 1, "https://www.aspose.com");
//Guardando el archivo Excel
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



