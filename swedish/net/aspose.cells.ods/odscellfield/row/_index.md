---
title: "OdsCellField.Row"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsCellField-egenskap. Hämtar och anger radindexet för cellen"
type: docs
url: /sv/net/aspose.cells.ods/odscellfield/row/
---
## OdsCellField.Row property

Hämtar och anger radindexet för cellen.

```csharp
public int Row { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;
            
            // Lägg till fält med olika typer
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 0, OdsCellFieldType.Title, null);
            
            odsCellFields.UpdateFieldsValue();

            // Demonstrera användning av Row-egenskapen
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                int row = field.Row; // Using Row property
                worksheet.Cells[row, 1].PutValue($"Row: {row}, Type: {field.FieldType}");
            }

            workbook.Save("OdsCellFieldRowDemo.ods");
        }
    }
}
```

### Se även

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


