---
title: "SaveOptions.CheckExcelRestriction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SaveOptions-Eigenschaft. Gibt an, ob die Beschränkungen einer Excel-Datei überprüft werden sollen, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht, einen Zeichenkettenwert einzugeben, der länger als 32 KB ist. Wenn Sie einen Wert eingeben, der länger als 32 KB ist, wird er abgeschnitten."
type: docs
url: /de/net/aspose.cells/saveoptions/checkexcelrestriction/
---
## SaveOptions.CheckExcelRestriction property

Ob die Beschränkungen der Excel-Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht, einen Zeichenfolgenwert länger als 32 KB einzugeben. Wenn Sie einen Wert eingeben, der länger als 32 KB ist, wird er abgeschnitten.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Excel-Beschränkungsprüfung deaktivieren
            workbook.Settings.CheckExcelRestriction = false;

            // Erste Arbeitsblatt und Zellen zugreifen
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Eine Zeichenkette erstellen, die länger ist als das normale Excel-Limit
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // Lange Zeichenkette in Zelle A1 einfügen
            cells["A1"].PutValue(longString);

            // Speicheroptionen konfigurieren, um Beschränkungen zu umgehen
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;

            // Speichere die Arbeitsmappe
            workbook.Save("output_without_restrictions.xlsx", saveOptions);

            // Gespeicherte Datei mit deaktivierten Beschränkungen laden
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output_without_restrictions.xlsx", loadOptions);

            // Überprüfen, ob die lange Zeichenkette erhalten geblieben ist
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("Loaded string length: " + loadedValue.Length);
            Console.WriteLine("First 50 chars: " + loadedValue.Substring(0, 50));
            Console.WriteLine("Last 50 chars: " + loadedValue.Substring(loadedValue.Length - 50));
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


