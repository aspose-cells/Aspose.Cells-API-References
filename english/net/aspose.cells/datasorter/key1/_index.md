---
title: DataSorter.Key1
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Represents first sorted column indexabsolute position column A is 0 B is 1 
type: docs
url: /net/aspose.cells/datasorter/key1/
---
## DataSorter.Key1 property

Represents first sorted column index(absolute position, column A is 0, B is 1, ...).

```csharp
public int Key1 { get; set; }
```

### Examples

```csharp
// Called: dataSorter.Key1 = 1;
[Test]
        public void Property_Key1()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Sort/TestDataSorter_134597.xls");
            DataSorter dataSorter = workbook.DataSorter;
            dataSorter.Key1 = 1;
            dataSorter.Order1 = SortOrder.Ascending;
            dataSorter.Key2 = 2;
            dataSorter.Order2 = SortOrder.Descending;

            CellArea area = new CellArea();
            {
                area.StartRow = 1;
                area.EndRow = 13;
                area.StartColumn = 1;
                area.EndColumn = 2;
            }
            dataSorter.Sort(workbook.Worksheets[0].Cells, area);
            Assert.AreEqual(workbook.Worksheets[0].Cells["C14"].StringValue, "7435.000");
        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


