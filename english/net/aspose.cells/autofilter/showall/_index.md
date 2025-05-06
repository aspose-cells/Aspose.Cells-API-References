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
[Test]
        public void Method_ShowAll()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;AutoFilter/555 RM_PP_Gas_Daily.xls&quot;);
            workbook.CalculateFormula();
            for (int i = 0; i &lt; workbook.Worksheets.Count; i++)
            {
                workbook.Worksheets[0].AutoFilter.ShowAll();
            }
            Util.ReSave(workbook, SaveFormat.Excel97To2003);//.Save(Constants.destPath + &quot;CellsNet14437.xls&quot;);
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


