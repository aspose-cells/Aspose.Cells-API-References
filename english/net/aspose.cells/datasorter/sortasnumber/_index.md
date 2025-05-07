---
title: DataSorter.SortAsNumber
second_title: Aspose.Cells for .NET API Reference
description: DataSorter property. Indicates whether sorting anything that looks like a number
type: docs
url: /net/aspose.cells/datasorter/sortasnumber/
---
## DataSorter.SortAsNumber property

Indicates whether sorting anything that looks like a number.

```csharp
public bool SortAsNumber { get; set; }
```

### Examples

```csharp
// Called: sorter.SortAsNumber = sortNumber;
private void Property_SortAsNumber(bool sortNumber)
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Sort/CellsNet45244.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            //Create your cell area 
            CellArea ca = CellArea.CreateCellArea("A1", "B4");

            //Create your sorter 
            DataSorter sorter = workbook.DataSorter;

            //Find the index, since we want to sort by column A, so we should know 
            //the index for sorter 
            int idx = CellsHelper.ColumnNameToIndex("A");

            //Add key in sorter, it will sort in Ascending order 
            sorter.AddKey(idx, SortOrder.Ascending);
            sorter.SortAsNumber = sortNumber;

            //Perform sort 
            sorter.Sort(worksheet.Cells, ca);
            if (sortNumber)
            {
                Assert.AreEqual(worksheet.Cells["A3"].StringValue,"21");
            }
            else
            {
                Assert.AreEqual(worksheet.Cells["A4"].StringValue, "21");
            }

            workbook.Save(Constants.destPath + "CellsNet45244.xlsx");
        }
```

### See Also

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


