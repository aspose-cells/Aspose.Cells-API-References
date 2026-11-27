---
title: "OdsCellField.Column"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsCellField-egenskap. Hämtar och anger kolumnindexet för cellen"
type: docs
url: /sv/net/aspose.cells.ods/odscellfield/column/
---
## OdsCellField.Column property

Hämtar och anger kolumnindexet för cellen.

```csharp
public int Column { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Lägg till fält med olika typer och demonstrera Column-egenskapen
            odsCellFields.Add(0, 2, OdsCellFieldType.Date, "yyyy-mm-dd");
            odsCellFields.Add(1, 3, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 4, OdsCellFieldType.Title, null);

            // Åtkomst till och visning av Column-egenskapen
            Console.WriteLine("Field Columns:");
            foreach (OdsCellField field in odsCellFields)
            {
                Console.WriteLine($"Type: {field.FieldType}, Column: {field.Column}");
                worksheet.Cells[field.Row, field.Column].PutValue($"Column: {field.Column}");
            }

            odsCellFields.UpdateFieldsValue();
            workbook.Save("OdsCellFieldColumnDemo.ods");
        }
    }
}
```

### Se även

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


