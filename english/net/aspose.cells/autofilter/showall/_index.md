---
title: AutoFilter.ShowAll
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Unhide all rows
type: docs
url: /net/aspose.cells/autofilter/showall/
---
## AutoFilter.ShowAll method

Unhide all rows.

```csharp
public void ShowAll()
```

### Examples

```csharp
// Called: workbook.Worksheets[0].AutoFilter.ShowAll();
public void AutoFilter_Method_ShowAll()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    workbook.CalculateFormula();
    for (int i = 0; i < workbook.Worksheets.Count; i++)
    {
        workbook.Worksheets[0].AutoFilter.ShowAll();
    }
    Util.ReSave(workbook, SaveFormat.Excel97To2003);//.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


