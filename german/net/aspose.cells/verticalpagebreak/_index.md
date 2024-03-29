---
title: VerticalPageBreak
second_title: Aspose.Cells für .NET-API-Referenz
description: Kapselt das Objekt das einen vertikalen Seitenumbruch darstellt.
type: docs
weight: 6310
url: /de/net/aspose.cells/verticalpagebreak/
---
## VerticalPageBreak class

Kapselt das Objekt, das einen vertikalen Seitenumbruch darstellt.

```csharp
public class VerticalPageBreak
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Column](../../aspose.cells/verticalpagebreak/column) { get; } | Ruft den Spaltenindex des vertikalen Seitenumbruchs ab. |
| [EndRow](../../aspose.cells/verticalpagebreak/endrow) { get; } | Ruft den Endzeilenindex des vertikalen Seitenumbruchs ab. |
| [StartRow](../../aspose.cells/verticalpagebreak/startrow) { get; } | Ruft den Startzeilenindex des vertikalen Seitenumbruchs ab. |

### Beispiele

```csharp
[C#]
Workbook excel = new Workbook();
//Seitenumbruch bei G5 hinzufügen
excel.Worksheets[0].HorizontalPageBreaks.Add("G5");
excel.Worksheets[0].VerticalPageBreaks.Add("G5");

[VB]
Dim excel as Workbook = new Workbook()
'Fügen Sie bei G5 einen Seitenumbruch hinzu
excel.Worksheets(0).HorizontalPageBreaks.Add("G5")
excel.Worksheets(0).VerticalPageBreaks.Add("G5")
```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
