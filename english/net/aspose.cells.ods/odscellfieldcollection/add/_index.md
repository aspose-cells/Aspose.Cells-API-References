---
title: OdsCellFieldCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: OdsCellFieldCollection method. Adds a field
type: docs
url: /net/aspose.cells.ods/odscellfieldcollection/add/
---
## OdsCellFieldCollection.Add method

Adds a field.

```csharp
public int Add(int row, int column, OdsCellFieldType fieldType, string format)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
| fieldType | OdsCellFieldType | The type of the field. |
| format | String | The number format of the field. |

### Examples

```csharp
// Called: int fieldIndex3 = odsCellFields.Add(2, 2, OdsCellFieldType.Title, null);
public static void Method_String_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Access the OdsCellFieldCollection
            OdsCellFieldCollection odsCellFields = cells.OdsCellFields;

            // Add fields to the OdsCellFieldCollection
            int fieldIndex1 = odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-MM-dd");
            int fieldIndex2 = odsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);
            int fieldIndex3 = odsCellFields.Add(2, 2, OdsCellFieldType.Title, null);

            // Update fields value to the cells
            odsCellFields.UpdateFieldsValue();

            // Save the workbook
            workbook.Save("OdsCellFieldCollectionExample.ods");

            return;
        }
```

### See Also

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


