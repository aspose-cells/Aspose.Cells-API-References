---
title: "SaveOptions.ClearData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SaveOptions-Eigenschaft. Macht die Arbeitsmappe nach dem Speichern der Datei leer."
type: docs
url: /de/net/aspose.cells/saveoptions/cleardata/
---
## SaveOptions.ClearData property

Die Arbeitsmappe nach dem Speichern der Datei leeren.

```csharp
public bool ClearData { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyClearDataDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Testdaten hinzu.
            worksheet.Cells["A1"].PutValue("Tabelle1");
            worksheet.Cells["B3"].PutValue(3);

            // Konfiguriere die Speicheroptionen mit ClearData = false
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.ClearData = false;
            saveOptions.Separator = ',';

            // Speichere die Arbeitsmappe
            string outputPath = "output_with_cleardata_false.csv";
            workbook.Save(outputPath, saveOptions);

            // Neu laden, um zu überprüfen, ob die Daten erhalten geblieben sind
            Workbook loadedWorkbook = new Workbook(outputPath);
            Cells cells = loadedWorkbook.Worksheets[0].Cells;
            
            Console.WriteLine("A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("B3 value: " + cells["B3"].IntValue);
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


