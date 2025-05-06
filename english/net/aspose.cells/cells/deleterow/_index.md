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
// Called: cells.DeleteRow(1048573);
[Test]
        public void Method_Int32_()
        {
            caseName = &quot;testDeleteRow_Excel2007_002&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[1048574, 0].PutValue(1);
            cells[1048574, 16383].PutValue(2);
            cells[1048575, 0].Formula = &quot;=A1&quot;;
            cells[1048575, 16383].PutValue(3);
            cells.DeleteRow(1048573);

            checkDeleteRow_Excel2007_002(workbook);
            workbook.Save(Constants.destPath + &quot;testDeleteRow.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testDeleteRow.xlsx&quot;);
            checkDeleteRow_Excel2007_002(workbook);
            workbook.Save(Constants.destPath + &quot;testDeleteRow.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot;testDeleteRow.xml&quot;);
            workbook.Save(Constants.destPath + &quot;testDeleteRow.xls&quot;);
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
            sheet.Cells[&quot;A1&quot;].PutValue(&quot;Item&quot;);
            sheet.Cells[&quot;A2&quot;].PutValue(&quot;Apple&quot;);
            sheet.Cells[&quot;A3&quot;].PutValue(&quot;Banana&quot;);
            sheet.Cells[&quot;A4&quot;].PutValue(&quot;Cherry&quot;);

            // Display the original data
            Console.WriteLine(&quot;Original Data:&quot;);
            for (int i = 1; i &lt;= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$&quot;A{i}&quot;].Value);
            }

            // Create DeleteOptions
            DeleteOptions options = new DeleteOptions
            {
                UpdateReference = true // Set to true to update references in other worksheets
            };

            // Delete the second row (Banana)
            sheet.Cells.DeleteRow(2, options.UpdateReference);

            // Display the data after deletion
            Console.WriteLine(&quot;\nData After Deletion:&quot;);
            for (int i = 1; i &lt;= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$&quot;A{i}&quot;].Value);
            }

            // Save the workbook
            workbook.Save(&quot;DeleteOptionsExample.xlsx&quot;);
            workbook.Save(&quot;DeleteOptionsExample.pdf&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


