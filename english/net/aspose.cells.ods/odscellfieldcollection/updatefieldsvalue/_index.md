---
title: OdsCellFieldCollection.UpdateFieldsValue
second_title: Aspose.Cells for .NET API Reference
description: OdsCellFieldCollection method. Update fields value to the cells
type: docs
url: /net/aspose.cells.ods/odscellfieldcollection/updatefieldsvalue/
---
## OdsCellFieldCollection.UpdateFieldsValue method

Update fields value to the cells.

```csharp
public void UpdateFieldsValue()
```

### Examples

```csharp
// Called: odsCellFields.UpdateFieldsValue();
public static void OdsCellFieldCollection_Method_UpdateFieldsValue()
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

* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


