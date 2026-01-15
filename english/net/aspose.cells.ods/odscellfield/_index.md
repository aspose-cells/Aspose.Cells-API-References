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
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Ods;

    public class OdsClassOdsCellFieldDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            try
            {
                // -----------------------------------------------------------------
                // 1. Create an OdsCellField via the collection (no parameterless ctor)
                // -----------------------------------------------------------------
                OdsCellFieldCollection odsFields = sheet.Cells.OdsCellFields;
                odsFields.Add(2, 1, OdsCellFieldType.Title, "Demo Title");

                // Retrieve the field we just added
                OdsCellField manualField = odsFields[odsFields.Count - 1];

                // Write something to the cell identified by the OdsCellField
                sheet.Cells[manualField.Row, manualField.Column].PutValue("Manual Field");

                // --------------------------------------------------------------
                // 2. Add the same field again to demonstrate collection usage (optional)
                // --------------------------------------------------------------
                odsFields.Add(manualField.Row, manualField.Column, manualField.FieldType, manualField.CustomFormat);

                // Update all ODS fields so they are reflected in the saved file
                odsFields.UpdateFieldsValue();

                // Display the property values to the console
                Console.WriteLine($"Created OdsCellField -> Row: {manualField.Row}, Column: {manualField.Column}, " +
                                  $"Type: {manualField.FieldType}, Format: {manualField.CustomFormat}");

                // Save the workbook as an ODS file
                workbook.Save("OdsClassOdsCellFieldDemo.ods");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with OdsCellField: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


