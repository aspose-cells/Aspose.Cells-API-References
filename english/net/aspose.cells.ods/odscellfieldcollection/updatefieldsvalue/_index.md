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
public static void Method_UpdateFieldsValue()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Create an OdsCellFieldCollection
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Add a new OdsCellField for the current date
            int rowIndex = 0;
            int columnIndex = 0;
            string customFormat = &quot;yyyy-mm-dd&quot;;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Date, customFormat);

            // Add another OdsCellField for the sheet name
            rowIndex = 1;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.SheetName, null);

            // Add another OdsCellField for the title
            rowIndex = 2;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Title, null);

            // Update the fields value to the cells
            odsCellFields.UpdateFieldsValue();

            // Output the values in the console
            for (int i = 0; i &lt; odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                worksheet.Cells[field.Row, field.Column].PutValue($&quot;Field Type: {field.FieldType}, Custom Format: {field.CustomFormat}&quot;);
            }

            // Save the workbook
            workbook.Save(&quot;OdsCellFieldTypeExample.ods&quot;);
        }
```

### See Also

* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


