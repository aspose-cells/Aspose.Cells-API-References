---
title: ThemeColor
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents a theme color.
type: docs
url: /fr/javascript-cpp/themecolor/
---

## ThemeColor class

Represents a theme color.

```javascript
class ThemeColor;
```


### Example
```javascript
const { Workbook, ThemeColor, ThemeColorType, BackgroundType, SaveFormat } = AsposeCells;

//Instanciation d'un objet Workbook
var workbook = new Workbook();
var cells = workbook.worksheets.get(0).cells;
cells.get("A1").putValue("Hello World");
var style = cells.get("A1").getStyle();
//Définir le type de couleur ThemeColorType.Text2 avec un éclaircissement de 40 % comme couleur de police.
style.font.themeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
style.pattern = BackgroundType.Solid;
//Définir le type de couleur ThemeColorType.Background2 avec un assombrissement de 75 % comme couleur de premier plan.
style.foregroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);
cells.get("A1").setStyle(style);
//Enregistrement du fichier Excel
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Constructors

| Name | Description |
| --- | --- |
| [constructor(ThemeColorType, number)](#constructor-themecolortype-number-)|  |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [colorType](#colorType--)| ThemeColorType | Gets and sets the theme type. |
| [tint](#tint--)| number | Gets and sets the tint value. |


### constructor(ThemeColorType, number) {#constructor-themecolortype-number-}



```javascript
constructor(type: ThemeColorType, tint: number);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ThemeColorType](../themecolortype/) | The theme type. |
| tint | number | The tint value. |

### colorType {#colorType--}

Gets and sets the theme type.

```javascript
colorType : ThemeColorType;
```


### tint {#tint--}

Gets and sets the tint value.

```javascript
tint : number;
```


**Remarks**

The tint value is stored as a double from -1.0 to 1.0, where -1.0 means 100% darken and 1.0 means 100% lighten. Also, 0.0 means no change.


