---
title: WorksheetCollection.GetNamedRangesAndTables
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Gets all predefined named ranges in the spreadsheet
type: docs
url: /net/aspose.cells/worksheetcollection/getnamedrangesandtables/
---
## WorksheetCollection.GetNamedRangesAndTables method

Gets all pre-defined named ranges in the spreadsheet.

```csharp
public Range[] GetNamedRangesAndTables()
```

### Return Value

An array of Range objects.

Returns null if the named range does not exist.

### Examples

```csharp
// Called: Aspose.Cells.Range[] ranges = workbook.Worksheets.GetNamedRangesAndTables(); //Error
public void WorksheetCollection_Method_GetNamedRangesAndTables()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "CL_IPD_Business_Plan_Template_Final_V2_BeforeCorruption.xlsm");
    Aspose.Cells.Range[] ranges = workbook.Worksheets.GetNamedRangesAndTables(); //Error
}
```

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


