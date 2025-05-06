---
title: CellsHelper.ColumnNameToIndex
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Gets column index according to column name
type: docs
url: /net/aspose.cells/cellshelper/columnnametoindex/
---
## CellsHelper.ColumnNameToIndex method

Gets column index according to column name.

```csharp
public static int ColumnNameToIndex(string columnName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| columnName | String | Column name. |

### Return Value

Column index.

### Examples

```csharp
// Called: int idx = CellsHelper.ColumnNameToIndex(&amp;quot;A&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA42266.xlsx&quot;);

            Worksheet worksheet = workbook.Worksheets[0];

            ////Create your cell area 
            CellArea ca = CellArea.CreateCellArea(&quot;A4&quot;, &quot;G18&quot;);

            //Create your sorter 
            DataSorter sorter = workbook.DataSorter;

            //Find the index, since we want to sort by column A, so we should know 
            //the index for sorter 
            int idx = CellsHelper.ColumnNameToIndex(&quot;A&quot;);

            //Add key in sorter, it will sort in Ascending order 
            sorter.AddKey(idx, SortOrder.Ascending);

            //Perform sort 
            sorter.Sort(worksheet.Cells, ca);

            Assert.AreEqual(&quot;C&quot;,workbook.Worksheets[0].Cells[&quot;F10&quot;].StringValue);
            Util.SaveManCheck(workbook, &quot;Shape&quot;, &quot;CELLSJAVA42266.xlsx&quot;);
        }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


