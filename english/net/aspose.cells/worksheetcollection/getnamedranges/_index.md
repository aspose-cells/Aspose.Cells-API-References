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
// Called: wb.Worksheets.GetNamedRanges();
public void WorksheetCollection_Method_GetNamedRanges()
{
    StringBuilder sb = null;
    for (int i = 1; i < 4; i++)
    {
        Workbook wb = new Workbook(Constants.sourcePath + "N42536_" + i + ".xlsx");
        try
        {
            wb.Worksheets.GetNamedRanges();
        }
        catch (Exception e)
        {
            if (sb == null)
            {
                sb = new StringBuilder();
                sb.Append("N42536_");
            }
            sb.Append(i);
            sb.Append(':');
            sb.Append(e.Message);
            sb.Append(';');
        }
    }
    if (sb != null)
    {
        AssertHelper.Fail(sb.ToString());
    }
}
```

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


