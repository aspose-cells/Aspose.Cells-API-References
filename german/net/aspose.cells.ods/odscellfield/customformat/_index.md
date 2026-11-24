---
title: "OdsCellField.CustomFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsCellField-Eigenschaft. Stellt das benutzerdefinierte Format des Feldwerts dar"
type: docs
url: /de/net/aspose.cells.ods/odscellfield/customformat/
---
## OdsCellField.CustomFormat property

Stellt das benutzerdefinierte Format des Feldwerts dar.

```csharp
public string CustomFormat { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyCustomFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;
            
            // Datumsfeld mit benutzerdefiniertem Format
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
            
            // Tabellennamenfeld ohne benutzerdefiniertes Format
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            
            // Titelfeld mit benutzerdefiniertem Format (demonstriert String-Format)
            odsCellFields.Add(2, 0, OdsCellFieldType.Title, "Title Format: @");
            
            odsCellFields.UpdateFieldsValue();
            
            foreach (OdsCellField field in odsCellFields)
            {
                worksheet.Cells[field.Row, field.Column].PutValue(
                    $"Type: {field.FieldType}, Format: {field.CustomFormat ?? "None"}");
            }
            
            workbook.Save("OdsCellFieldCustomFormatDemo.ods");
        }
    }
}
```

### Siehe auch

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


