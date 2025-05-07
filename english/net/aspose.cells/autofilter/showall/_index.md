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
// Called: wSheet.AutoFilter.ShowAll();
[Test]
        public void Method_ShowAll()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "AutoFilter/CellsNet48512.xlsx");
            Worksheet wSheet = workbook.Worksheets[0];
            if (wSheet.HasAutofilter)
            {
                Console.WriteLine("Autofilter detected");
                int[] rows = wSheet.AutoFilter.Refresh(false);//It shows correct row numbers that are hidden due to filter
                wSheet.AutoFilter.ShowAll();
                int[] rows2 = wSheet.AutoFilter.Refresh(false);//It shows correct result as null
            }
            Assert.IsFalse(wSheet.Cells.IsRowHidden(13));
            Assert.IsFalse(wSheet.Cells.IsRowHidden(15));
            //.Save(Constants.destPath + "CellsNet48512.xlsx");//In the output file rows containing value 2 are missing
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


