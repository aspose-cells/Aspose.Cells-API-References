---
title: WorksheetCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Clear all worksheets
type: docs
url: /net/aspose.cells/worksheetcollection/clear/
---
## WorksheetCollection.Clear method

Clear all worksheets.

```csharp
public void Clear()
```

### Remarks

A workbook must contains a worksheet.

### Examples

```csharp
// Called: workbook.Worksheets.Clear();
public static void WorksheetCollection_Method_Clear(Workbook workbook, bool IsGridlinesVisible, params string[] sheetNames)
        {
            workbook.Worksheets.Clear();
            foreach (string str in sheetNames)
            {
                workbook.Worksheets.Add(str);
                workbook.Worksheets[str].IsGridlinesVisible = IsGridlinesVisible;
            }
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


