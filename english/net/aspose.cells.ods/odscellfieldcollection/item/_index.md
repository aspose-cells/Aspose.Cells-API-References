---
title: OdsCellFieldCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: OdsCellFieldCollection property. Gets the field by the index
type: docs
url: /net/aspose.cells.ods/odscellfieldcollection/item/
---
## OdsCellFieldCollection indexer (1 of 2)

Gets the field by the index.

```csharp
public OdsCellField this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add ODS cell fields with format parameter
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "");
            sheet.Cells.OdsCellFields.Add(0, 1, OdsCellFieldType.SheetName, "");

            // Access fields using Item property
            OdsCellField titleField = sheet.Cells.OdsCellFields[0];
            OdsCellField sheetNameField = sheet.Cells.OdsCellFields[1];

            // Output field types
            Console.WriteLine("Field 0 Type: " + titleField.FieldType);
            Console.WriteLine("Field 1 Type: " + sheetNameField.FieldType);

            // Save and reload
            workbook.Save("output.ods");
            workbook = new Workbook("output.ods");
            sheet = workbook.Worksheets[0];

            // Verify persisted fields
            Console.WriteLine("Reloaded Field 0 Type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("Reloaded Field 1 Type: " + sheet.Cells.OdsCellFields[1].FieldType);
        }
    }
}
```

### See Also

* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)

---

## OdsCellFieldCollection indexer (2 of 2)

Gets the field by row and column index.

```csharp
public OdsCellField this[int row, int column] { get; }
```

| Parameter | Description |
| --- | --- |
| row | The row index. |
| column | The column index. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsCellFieldCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Get the OdsCellFieldCollection from the worksheet
            OdsCellFieldCollection fieldCollection = worksheet.Cells.OdsCellFields;

            // Add fields to the collection
            int index1 = fieldCollection.Add(0, 0, OdsCellFieldType.Date, "yyyy-MM-dd");
            int index2 = fieldCollection.Add(1, 1, OdsCellFieldType.Title, "$#,##0.00");

            // Access items using the Item property
            OdsCellField field1 = fieldCollection[index1];
            OdsCellField field2 = fieldCollection[index2];

            // Display field information
            Console.WriteLine("Field 1 - Row: {0}, Column: {1}, Type: {2}, Format: {3}", 
                field1.Row, field1.Column, field1.FieldType, field1.CustomFormat);
            Console.WriteLine("Field 2 - Row: {0}, Column: {1}, Type: {2}, Format: {3}", 
                field2.Row, field2.Column, field2.FieldType, field2.CustomFormat);

            // Update fields value to the cells
            fieldCollection.UpdateFieldsValue();

            // Save the result
            workbook.Save("OdsCellFieldCollectionDemo.ods");
        }
    }
}
```

### See Also

* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


