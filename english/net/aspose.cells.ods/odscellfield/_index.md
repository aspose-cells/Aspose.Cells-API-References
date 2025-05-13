---
title: Class OdsCellField
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Ods.OdsCellField class. Represents the cell field of ods
type: docs
url: /net/aspose.cells.ods/odscellfield/
---
## OdsCellField class

Represents the cell field of ods.

```csharp
public class OdsCellField
```

## Properties

| Name | Description |
| --- | --- |
| [Column](../../aspose.cells.ods/odscellfield/column/) { get; set; } | Get and sets the column index of the cell. |
| [CustomFormat](../../aspose.cells.ods/odscellfield/customformat/) { get; set; } | Represents the custom format of the field's value. |
| [FieldType](../../aspose.cells.ods/odscellfield/fieldtype/) { get; set; } | Gets and sets the type of the field. |
| [Row](../../aspose.cells.ods/odscellfield/row/) { get; set; } | Get and sets the row index of the cell. |

### Examples

```csharp
// Called: OdsCellField field = odsCellFields[i];
public static void Ods_Type_OdsCellField()
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

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


