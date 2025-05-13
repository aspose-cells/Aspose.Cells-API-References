---
title: Cells.DeleteRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Deletes a row
type: docs
url: /net/aspose.cells/cells/deleterow/
---
## DeleteRow(int) {#deleterow}

Deletes a row.

```csharp
public void DeleteRow(int rowIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index of the row to be deleted. |

### Examples

```csharp
// Called: cells.DeleteRow(9);
public void Cells_Method_DeleteRow()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    cells[66, 1].SetSharedFormula("=SUM(B10:B66)", 1, 6);
    cells.DeleteRow(9);
    for (int i = 1; i < 7; i++)
    {
        char cn = (char)('A' + i);
        Assert.AreEqual("=SUM(" + cn + "10:" + cn + "65)", cells[65, i].Formula, cn + "67->" + cn + "66");
    }
    cells.DeleteRows(60, 2);
    for (int i = 1; i < 7; i++)
    {
        char cn = (char) ('A' + i);
        Assert.AreEqual("=SUM(" + cn + "10:" + cn + "63)", cells[63, i].Formula, cn + "67->" + cn + "64");
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRow(int, bool) {#deleterow_1}

Deletes a row.

```csharp
public void DeleteRow(int rowIndex, bool updateReference)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Index of the row to be deleted. |
| updateReference | Boolean | Indicates whether update references in other worksheets. |

### Examples

```csharp
// Called: sheet.Cells.DeleteRow(2, options.UpdateReference);
public static void Cells_Method_DeleteRow()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            // Display the original data
            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Create DeleteOptions
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Set to true to update references in other worksheets
            };

            // Delete the second row (Banana)
            sheet.Cells.DeleteRow(2, options.UpdateReference);

            // Display the data after deletion
            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            // Save the workbook
            workbook.Save("DeleteOptionsExample.xlsx");
            workbook.Save("DeleteOptionsExample.pdf");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


