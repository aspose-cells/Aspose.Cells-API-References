---
title: FontSetting
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents a range of characters within the cell text.
type: docs
url: /tr/javascript-cpp/fontsetting/
---

## FontSetting class

Represents a range of characters within the cell text.

```javascript
class FontSetting;
```


### Example
```javascript
const { Workbook, Color, SaveFormat } = AsposeCells;

//Bir Workbook nesnesi oluşturma
var workbook = new Workbook();
//Excel nesnesine yeni bir çalışma sayfası ekleme
workbook.worksheets.add();
//Yeni eklenen çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
var worksheet = workbook.worksheets.get(0);
//"A1" hücresine çalışma sayfasından erişme
var cell = worksheet.cells.get("A1");
//"A1" hücresine bir değer ekleme
cell.putValue("Visit Aspose!");
//karakter alınıyor
var charactor = cell.characters(6, 7);
//Seçili karakterlerin yazı tipini kalın olarak ayarlama
charactor.font.isBold = true;
//Seçili karakterlerin yazı tipi rengini mavi olarak ayarlama
charactor.font.color = Color.Blue;
//Excel dosyasını kaydetme
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Constructors

| Name | Description |
| --- | --- |
| [constructor(number, number, WorksheetCollection)](#constructor-number-number-worksheetcollection-)|  |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [startIndex](#startIndex--)| number | Readonly. Gets the start index of the characters. |
| [length](#length--)| number | Readonly. Gets the length of the characters. |
| [font](#font--)| Font | Readonly. Returns the font of this object. |
| [textOptions](#textOptions--)| TextOptions | Readonly. Returns the text options. |

## Methods

| Method | Description |
| --- | --- |
| [setWordArtStyle(PresetWordArtStyle)](#setWordArtStyle-presetwordartstyle-)| Sets the preset WordArt style. |
| [getType()](#getType--)| Gets the type of text node. |


### constructor(number, number, WorksheetCollection) {#constructor-number-number-worksheetcollection-}



```javascript
constructor(startIndex: number, length: number, sheets: WorksheetCollection);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number |  |
| length | number |  |
| sheets | [WorksheetCollection](../worksheetcollection/) |  |

### startIndex {#startIndex--}

Readonly. Gets the start index of the characters.

```javascript
startIndex : number;
```


### length {#length--}

Readonly. Gets the length of the characters.

```javascript
length : number;
```


### font {#font--}

Readonly. Returns the font of this object.

```javascript
font : Font;
```


### textOptions {#textOptions--}

Readonly. Returns the text options.

```javascript
textOptions : TextOptions;
```


### setWordArtStyle(PresetWordArtStyle) {#setWordArtStyle-presetwordartstyle-}

Sets the preset WordArt style.

```javascript
setWordArtStyle(style: PresetWordArtStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [PresetWordArtStyle](../presetwordartstyle/) | The preset WordArt style. |

**Remarks**

Only for the text of shape/chart.

### getType() {#getType--}

Gets the type of text node.

```javascript
getType() : TextNodeType;
```


**Returns**

[TextNodeType](../textnodetype/)


