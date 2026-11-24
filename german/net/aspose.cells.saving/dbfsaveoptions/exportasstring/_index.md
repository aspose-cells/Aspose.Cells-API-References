---
title: "DbfSaveOptions.ExportAsString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DbfSaveOptions‑Eigenschaft. Gibt an, ob als Zeichenkettenwert exportiert wird"
type: docs
url: /de/net/aspose.cells.saving/dbfsaveoptions/exportasstring/
---
## DbfSaveOptions.ExportAsString property

Gibt an, ob als Zeichenkettenwert exportiert wird

```csharp
public bool ExportAsString { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit gemischten Typen hinzufügen
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("TextValue");

            // Erstelle DbfSaveOptions-Instanz
            DbfSaveOptions options = new DbfSaveOptions();

            // Aktuellen ExportAsString-Wert anzeigen
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // Setze ExportAsString auf true (alle Werte werden als Zeichenketten exportiert)
            options.ExportAsString = true;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // Speichern mit ExportAsString = true
            workbook.Save("ExportAsStringTrue.dbf", options);

            // Setze ExportAsString auf false (Werte behalten ihre ursprünglichen Typen bei)
            options.ExportAsString = false;
            Console.WriteLine("ExportAsString set to: " + options.ExportAsString);

            // Speichern mit ExportAsString = false
            workbook.Save("ExportAsStringFalse.dbf", options);
        }
    }
}
```

### Siehe auch

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


