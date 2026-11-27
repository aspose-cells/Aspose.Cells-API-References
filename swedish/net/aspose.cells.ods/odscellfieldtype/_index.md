---
title: "Enum OdsCellFieldType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Ods.OdsCellFieldType enum. Representerar cellfältstypen för ods"
type: docs
url: /sv/net/aspose.cells.ods/odscellfieldtype/
---
## OdsCellFieldType enumeration

Representerar cellfälttypen för ods.

```csharp
public enum OdsCellFieldType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Date | `0` | Aktuellt datum. |
| SheetName | `1` | Namnet på bladet. |
| Title | `2` | Namnet på filen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsCellFieldTypeDemo
    {
        public static void OdsCellFieldTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en OdsCellFieldCollection
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Lägg till ett nytt OdsCellField för det aktuella datumet
            int rowIndex = 0;
            int columnIndex = 0;
            string customFormat = "yyyy-mm-dd";
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Date, customFormat);

            // Lägg till ett annat OdsCellField för bladnamnet
            rowIndex = 1;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.SheetName, null);

            // Lägg till ett annat OdsCellField för titeln
            rowIndex = 2;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Title, null);

            // Uppdatera fältens värde till cellerna
            odsCellFields.UpdateFieldsValue();

            // Skriv ut värdena i konsolen
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                worksheet.Cells[field.Row, field.Column].PutValue($"Field Type: {field.FieldType}, Custom Format: {field.CustomFormat}");
            }

            // Spara arbetsboken
            workbook.Save("OdsCellFieldTypeExample.ods");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


