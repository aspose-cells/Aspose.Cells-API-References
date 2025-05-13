---
title: OdsCellField.CustomFormat
second_title: Aspose.Cells for .NET API Reference
description: OdsCellField property. Represents the custom format of the fields value
type: docs
url: /net/aspose.cells.ods/odscellfield/customformat/
---
## OdsCellField.CustomFormat property

Represents the custom format of the field's value.

```csharp
public string CustomFormat { get; set; }
```

### Examples

```csharp
// Called: worksheet.Cells[field.Row, field.Column].PutValue($"Field Type: {field.FieldType}, Custom Format: {field.CustomFormat}");
public static void OdsCellField_Property_CustomFormat()
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
            string customFormat = "yyyy-mm-dd";
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
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                worksheet.Cells[field.Row, field.Column].PutValue($"Field Type: {field.FieldType}, Custom Format: {field.CustomFormat}");
            }

            // Save the workbook
            workbook.Save("OdsCellFieldTypeExample.ods");
        }
```

### See Also

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


