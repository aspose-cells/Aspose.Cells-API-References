---
title: "OdsCellField.FieldType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsCellField-egenskap. Hämtar och anger fältets typ"
type: docs
url: /sv/net/aspose.cells.ods/odscellfield/fieldtype/
---
## OdsCellField.FieldType property

Hämtar och anger typen för fältet.

```csharp
public OdsCellFieldType FieldType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyFieldTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till ODS-cellfält med olika fälttyper och formatsträngar
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "Title Format");
            sheet.Cells.OdsCellFields.Add(1, 0, OdsCellFieldType.SheetName, "SheetName Format");

            // Demonstrera användning av FieldType-egenskapen
            Console.WriteLine("Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);

            // Spara och ladda om för att demonstrera beständighet
            workbook.Save("output.ods");
            workbook = new Workbook("output.ods");
            sheet = workbook.Worksheets[0];

            // Verifiera FieldType efter omladdning
            Console.WriteLine("After reload - Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("After reload - Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);
        }
    }
}
```

### Se även

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


