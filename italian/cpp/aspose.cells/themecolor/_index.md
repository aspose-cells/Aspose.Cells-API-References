---
title: Aspose::Cells::ThemeColor class
linktitle: ThemeColor
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::ThemeColor class. Represents a theme color in C++.'
type: docs
weight: 14700
url: /it/cpp/aspose.cells/themecolor/
---
## ThemeColor class


Represents a theme color.

```cpp
class ThemeColor
```

## Methods

| Method | Description |
| --- | --- |
| [GetColorType()](./getcolortype/) | Gets and sets the theme type. |
| [GetTint()](./gettint/) | Gets and sets the tint value. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ThemeColor\& src)](./operator_asm/) | operator= |
| [SetColorType(ThemeColorType value)](./setcolortype/) | Gets and sets the theme type. |
| [SetTint(double value)](./settint/) | Gets and sets the tint value. |
| [ThemeColor(ThemeColorType type, double tint)](./themecolor/) |  |
| [ThemeColor(ThemeColor_Impl* impl)](./themecolor/) | Constructs from an implementation object. |
| [ThemeColor(const ThemeColor\& src)](./themecolor/) | Copy constructor. |
| [~ThemeColor()](./~themecolor/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |

## Examples


```cpp
Aspose::Cells::Startup();
//Istanziare un oggetto Workbook
Workbook workbook;
Cells cells = workbook.GetWorksheets().Get(0).GetCells();
cells.Get(u"A1").PutValue(u"Hello World");
Style style = cells.Get(u"A1").GetStyle();
//Imposta il tipo di colore ThemeColorType.Text2 con un chiarimento del 40% come colore del carattere.
style.GetFont().SetThemeColor(ThemeColor(ThemeColorType::Text2, 0.4));
style.SetPattern(BackgroundType::Solid);
//Imposta il tipo di colore ThemeColorType.Background2 con un'oscuramento del 75% come colore di primo piano
style.SetForegroundThemeColor(ThemeColor(ThemeColorType::Background2, -0.75));
cells.Get(u"A1").SetStyle(style);
//Salvataggio del file Excel
workbook.Save(u"book1.xlsx");

Aspose::Cells::Cleanup();
```

## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
