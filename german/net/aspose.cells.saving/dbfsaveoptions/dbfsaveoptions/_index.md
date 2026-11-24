---
title: "DbfSaveOptions.DbfSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DbfSaveOptions‑Konstruktor. Die Optionen zum Speichern einer .dbf‑Datei"
type: docs
url: /de/net/aspose.cells.saving/dbfsaveoptions/dbfsaveoptions/
---
## DbfSaveOptions constructor

Die Optionen zum Speichern einer .dbf-Datei.

```csharp
public DbfSaveOptions()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class DbfSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // Erstelle eine DbfSaveOptions‑Instanz mit dem Konstruktor
                DbfSaveOptions saveOptions = new DbfSaveOptions();
                
                // Setze Eigenschaften der Speicheroptionen
                saveOptions.ExportAsString = true;
                
                // Speichere die Arbeitsmappe mit DBF-Speicheroptionen
                workbook.Save("DbfSaveOptionsDemo.dbf", saveOptions);
                
                Console.WriteLine("DBF file saved successfully with ExportAsString option set to true");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving DBF file: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [DbfSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


