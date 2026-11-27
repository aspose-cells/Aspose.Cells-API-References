---
title: "OdsCellField.CustomFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsCellField-egenskap. Representerar det anpassade formatet för fältets värde"
type: docs
url: /sv/net/aspose.cells.ods/odscellfield/customformat/
---
## OdsCellField.CustomFormat property

Representerar det anpassade formatet för fältets värde.

```csharp
public string CustomFormat { get; set; }
```

### Exempel

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
            
            // Datumfält med anpassat format
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
            
            // Bladnamnsfält utan anpassat format
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            
            // Titel-fält med anpassat format (demonstrerar strängformat)
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

### Se även

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


