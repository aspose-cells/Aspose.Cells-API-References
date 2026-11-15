---
title: Aspose::Cells::WorkbookSettings::IsHScrollBarVisible method
linktitle: IsHScrollBarVisible
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::WorkbookSettings::IsHScrollBarVisible method. Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar in C++.'
type: docs
weight: 2500
url: /es/cpp/aspose.cells/workbooksettings/ishscrollbarvisible/
---
## WorkbookSettings::IsHScrollBarVisible method


Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar.

```cpp
bool Aspose::Cells::WorkbookSettings::IsHScrollBarVisible()
```

## Remarks


The default value is true.

## Examples


```cpp
//El siguiente código hace que la barra de desplazamiento horizontal sea invisible para la hoja de cálculo.
// Ocultar la barra de desplazamiento horizontal del archivo Excel.
if (settings.IsHScrollBarVisible())
{
    settings.SetIsHScrollBarVisible(false);
}
```

## See Also

* Class [Vector](../../vector/)
* Class [WorkbookSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
