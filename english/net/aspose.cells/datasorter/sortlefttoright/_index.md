---
title: DataSorter.SortLeftToRight
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false
type: docs
url: /net/aspose.cells/datasorter/sortlefttoright/
---
## DataSorter.SortLeftToRight property

True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false.

```csharp
public bool SortLeftToRight { get; set; }
```

### Examples

```csharp
// Called: dataSorter.SortLeftToRight = true;
[Test]
        public void Property_SortLeftToRight()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Sort/TestLeftToRight_001.xls&quot;);
            DataSorter dataSorter = workbook.DataSorter;

            dataSorter.Key1 = 0;
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 2;
            dataSorter.SortLeftToRight = true;
            dataSorter.Sort(workbook.Worksheets[0].Cells, area);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;A1&quot;].DoubleValue, 4);
            workbook.Save(Constants.destPath + &quot;TestLeftToRight_001.xls&quot;);

        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


