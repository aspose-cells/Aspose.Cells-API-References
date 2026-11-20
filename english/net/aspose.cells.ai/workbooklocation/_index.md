---
title: Class WorkbookLocation
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.WorkbookLocation class. A structured value object that identifies a part of a workbook: a worksheet, a cell, a range, a ListObject (table) or a defined name."
type: docs
url: /net/aspose.cells.ai/workbooklocation/
---
## WorkbookLocation class

A structured value object that identifies a part of a workbook: a worksheet, a cell, a range, a ListObject (table) or a defined name.

```csharp
public sealed class WorkbookLocation : IEquatable<WorkbookLocation>
```

## Properties

| Name | Description |
| --- | --- |
| [Address](address/) { get; } | The A1 address. Only for Cell and Range. |
| [Kind](kind/) { get; } | Gets the kind of this location. |
| [Name](name/) { get; } | The name. Only for Table and DefinedName. |
| [Reference](reference/) { get; } | A display string for the location. Used only for presentation and logging; internal implementation must not re-parse Reference to resolve a location. |
| [WorksheetName](worksheetname/) { get; } | The worksheet name. Null for workbook-scoped defined names. |

## Methods

| Name | Description |
| --- | --- |
| [Equals](equals/#equals)(Object) | Determines whether the specified object is equal to the current object. |
| [Equals](equals/#equals_1)(WorkbookLocation) | Determines whether the specified WorkbookLocation is equal to the current object. |
| static [FromCell](fromcell/)(String, String) | Creates a location identifying a single cell by A1 address. |
| static [FromDefinedName](fromdefinedname/#fromdefinedname)(String) | Creates a workbook-scoped defined name location. |
| static [FromDefinedName](fromdefinedname/#fromdefinedname_1)(String, String) | Creates a worksheet-scoped defined name location. |
| static [FromRange](fromrange/)(String, String) | Creates a location identifying a rectangular range by A1 address. |
| static [FromTable](fromtable/)(String, String) | Creates a location identifying a ListObject (Excel table) by name. |
| static [FromWorksheet](fromworksheet/)(String) | Creates a location identifying a worksheet by name. |
| [GetHashCode](gethashcode/)() | Returns a hash code for the current object. |
| [ToString](tostring/)() | Returns a string that represents the current object. |

### See Also

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../)
