---
title: ListObject.ConvertToRange
second_title: Aspose.Cells for .NET API Reference
description: ListObject method. Convert the table to range
type: docs
url: /net/aspose.cells.tables/listobject/converttorange/
---
## ConvertToRange() {#converttorange}

Convert the table to range.

```csharp
public void ConvertToRange()
```

### Examples

```csharp
// Called: sheet.ListObjects[i].ConvertToRange();
public void ListObject_Method_ConvertToRange()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    foreach (Worksheet sheet in workbook.Worksheets)
    {
        for (int i = 0; i < sheet.ListObjects.Count; i++)
        {
            sheet.ListObjects[i].ConvertToRange();

        }
    }

}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## ConvertToRange(TableToRangeOptions) {#converttorange_1}

Convert the table to range.

```csharp
public void ConvertToRange(TableToRangeOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | TableToRangeOptions | the options when converting table to range. |

### Examples

```csharp
// Called: table.ConvertToRange(options);
public static void ListObject_Method_ConvertToRange()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Populate the worksheet with some data
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Add a ListObject (table) to the worksheet
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Set some properties of the table
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;

            // Create an instance of TableToRangeOptions
            TableToRangeOptions options = new TableToRangeOptions
            {
                LastRow = 9 // Set the last row index of the table
            };

            // Convert the table to a range using the options
            table.ConvertToRange(options);

            // Save the workbook
            workbook.Save("TableToRangeOptionsExample.xlsx");
        }
```

### See Also

* class [TableToRangeOptions](../../tabletorangeoptions/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


