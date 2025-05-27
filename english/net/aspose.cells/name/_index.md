---
title: Class Name
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Name class. Represents a defined name for a range of cells
type: docs
url: /net/aspose.cells/name/
---
## Name class

Represents a defined name for a range of cells.

```csharp
public class Name
```

## Properties

| Name | Description |
| --- | --- |
| [Comment](../../aspose.cells/name/comment/) { get; set; } | Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions. |
| [FullText](../../aspose.cells/name/fulltext/) { get; } | Gets the name full text of the object with the scope setting. |
| [IsReferred](../../aspose.cells/name/isreferred/) { get; } | Indicates whether this name is referred by other formulas. |
| [IsVisible](../../aspose.cells/name/isvisible/) { get; set; } | Indicates whether the name is visible. |
| [R1C1RefersTo](../../aspose.cells/name/r1c1refersto/) { get; set; } | Gets or sets a R1C1 reference of the `Name`. |
| [RefersTo](../../aspose.cells/name/refersto/) { get; set; } | Returns or sets the formula that the name is defined to refer to, beginning with an equal sign. |
| [SheetIndex](../../aspose.cells/name/sheetindex/) { get; set; } | Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based) |
| [Text](../../aspose.cells/name/text/) { get; set; } | Gets the name text of the object. |

## Methods

| Name | Description |
| --- | --- |
| [GetRange](../../aspose.cells/name/getrange/#getrange)() | Gets the range if this name refers to a range. |
| [GetRange](../../aspose.cells/name/getrange/#getrange_1)(bool) | Gets the range if this name refers to a range |
| [GetRange](../../aspose.cells/name/getrange/#getrange_2)(int, int, int) | Gets the range if this name refers to a range. If the reference of this name is not absolute, the range may be different for different cell. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges)() | Gets all ranges referred by this name. |
| [GetRanges](../../aspose.cells/name/getranges/#getranges_1)(bool) | Gets all ranges referred by this name. |
| [GetReferredAreas](../../aspose.cells/name/getreferredareas/)(bool) | Gets all references referred by this name. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto)(bool, bool) | Get the reference of this Name. |
| [GetRefersTo](../../aspose.cells/name/getrefersto/#getrefersto_1)(bool, bool, int, int) | Get the reference of this Name based on specified cell. |
| [SetRefersTo](../../aspose.cells/name/setrefersto/)(string, bool, bool) | Set the reference of this Name. |
| override [ToString](../../aspose.cells/name/tostring/)() | Returns a string represents the current Range object. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B4", "G14");
            range.Name = "TestRange";
            workbook.Save("output.xls");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


