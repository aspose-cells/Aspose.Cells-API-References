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
// Called: cells.DeleteRow(1);
[Test]
        public void Method_Int32_()
        {
            caseName = "testDeleteFormual_002";
            Workbook workbook = new Workbook();
            workbook = new Workbook(Constants.sourcePath + "insertDelete\\testformual.xls");
            Cells cells = workbook.Worksheets[0].Cells;
            cells.DeleteRow(1);

            checkDeleteFormual_002(workbook);
            workbook.Save(Constants.destPath + "testDeleteFormual.xls");
            workbook = new Workbook(Constants.destPath + "testDeleteFormual.xls");
            checkDeleteFormual_002(workbook);
            workbook.Save(Constants.destPath + "testDeleteFormual.xlsx");
            workbook = new Workbook(Constants.destPath + "testDeleteFormual.xlsx");
            checkDeleteFormual_002(workbook);
            workbook.Save(Constants.destPath + "testDeleteFormual.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testDeleteFormual.xml");
            checkDeleteFormual_002(workbook);
            workbook.Save(Constants.destPath + "testDeleteFormual.xls");
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
public static void Method_Boolean_()
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


