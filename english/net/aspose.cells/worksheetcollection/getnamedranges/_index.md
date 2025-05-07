---
title: WorksheetCollection.GetNamedRanges
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Gets all predefined named ranges in the spreadsheet
type: docs
url: /net/aspose.cells/worksheetcollection/getnamedranges/
---
## WorksheetCollection.GetNamedRanges method

Gets all pre-defined named ranges in the spreadsheet.

```csharp
public Range[] GetNamedRanges()
```

### Return Value

An array of Range objects. If the defined Name's reference is external or has multiple ranges, no Range object will be returned for this Name.

Returns null if the named range does not exist.

### Examples

```csharp
// Called: Aspose.Cells.Range[] rs = workbook.Worksheets.GetNamedRanges();
[Test]
        public void Method_GetNamedRanges()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet40596.xls");
            Aspose.Cells.Range[] rs = workbook.Worksheets.GetNamedRanges();
            workbook = new Workbook(Constants.sourcePath + "CellsNet40596.xlsm");
           rs = workbook.Worksheets.GetNamedRanges();
        }
```

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


