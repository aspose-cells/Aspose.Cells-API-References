---
title: "OdsCellFieldCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsCellFieldCollection egenskap. Hämtar fältet efter indexet"
type: docs
url: /sv/net/aspose.cells.ods/odscellfieldcollection/item/
---
## OdsCellFieldCollection indexer (1 of 2)

Hämtar fältet efter indexet.

```csharp
public OdsCellField this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till ODS-cellfält med formatparameter
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "");
            sheet.Cells.OdsCellFields.Add(0, 1, OdsCellFieldType.SheetName, "");

            // Kom åt fält med Item-egenskapen
            OdsCellField titleField = sheet.Cells.OdsCellFields[0];
            OdsCellField sheetNameField = sheet.Cells.OdsCellFields[1];

            // Skriv ut fälttyper
            Console.WriteLine("Field 0 Type: " + titleField.FieldType);
            Console.WriteLine("Field 1 Type: " + sheetNameField.FieldType);

            // Spara och ladda om
            workbook.Save("output.ods");
            workbook = new Workbook("output.ods");
            sheet = workbook.Worksheets[0];

            // Verifiera beständiga fält
            Console.WriteLine("Reloaded Field 0 Type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("Reloaded Field 1 Type: " + sheet.Cells.OdsCellFields[1].FieldType);
        }
    }
}
```

### Se även

* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)

---

## OdsCellFieldCollection indexer (2 of 2)

Hämtar fältet efter rad- och kolumnindex.

```csharp
public OdsCellField this[int row, int column] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| row | Radindexet. |
| column | Kolumnindexet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till några ODS-cellfält
            // (rad, kolumn, fälttyp, format)
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "TitleFormat");
            sheet.Cells.OdsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);

            try
            {
                // Kom åt fält med Item-egenskapen (indexerare)
                // 1) Efter samlingsindex
                OdsCellField firstField = sheet.Cells.OdsCellFields[0];
                Console.WriteLine("First field type (by index): " + firstField.FieldType);

                // 2) Efter cellposition (rad, kolumn)
                OdsCellField titleField = sheet.Cells.OdsCellFields[0, 0];
                Console.WriteLine("Field at (0,0) type (by position): " + titleField.FieldType);

                // Uppdatera cellerna med fältvärdena
                sheet.Cells.OdsCellFields.UpdateFieldsValue();

                // Spara arbetsboken (ODS-format bevarar fälten)
                workbook.Save("OdsCellFieldItemDemo.ods");
                Console.WriteLine("Workbook saved as OdsCellFieldItemDemo.ods");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Se även

* class [OdsCellField](../../odscellfield/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


