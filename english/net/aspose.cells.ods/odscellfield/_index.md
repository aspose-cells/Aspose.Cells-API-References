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
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsClassOdsCellFieldDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Add date field with custom format
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-MM-dd");
            
            // Add sheet name field
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            
            // Add title field
            odsCellFields.Add(2, 0, OdsCellFieldType.Title, null);

            // Update all fields
            odsCellFields.UpdateFieldsValue();

            // Save the workbook
            workbook.Save("OdsCellFieldDemo.ods");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


