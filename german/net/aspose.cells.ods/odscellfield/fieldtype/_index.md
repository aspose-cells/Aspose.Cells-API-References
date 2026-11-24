---
title: "OdsCellField.FieldType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsCellField-Eigenschaft. Liest und setzt den Typ des Feldes"
type: docs
url: /de/net/aspose.cells.ods/odscellfield/fieldtype/
---
## OdsCellField.FieldType property

Liest und schreibt den Typ des Feldes.

```csharp
public OdsCellFieldType FieldType { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // ODS-Zellfelder mit unterschiedlichen Feldtypen und Formatzeichenketten hinzufügen
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "Title Format");
            sheet.Cells.OdsCellFields.Add(1, 0, OdsCellFieldType.SheetName, "SheetName Format");

            // Verwendung der FieldType-Eigenschaft demonstrieren
            Console.WriteLine("Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);

            // Speichern und neu laden, um die Persistenz zu demonstrieren
            workbook.Save("output.ods");
            workbook = new Workbook("output.ods");
            sheet = workbook.Worksheets[0];

            // FieldType nach dem Neuladen überprüfen
            Console.WriteLine("After reload - Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("After reload - Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);
        }
    }
}
```

### Siehe auch

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


