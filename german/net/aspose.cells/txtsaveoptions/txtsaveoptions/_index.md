---
title: "TxtSaveOptions.TxtSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtSaveOptions-Konstruktor. Erstellt Optionen zum Speichern von Textdateien"
type: docs
url: /de/net/aspose.cells/txtsaveoptions/txtsaveoptions/
---
## TxtSaveOptions() {#constructor}

Erstellt Optionen zum Speichern von Textdateien.

```csharp
public TxtSaveOptions()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            
            // Demonstriere den TxtSaveOptions-Konstruktor
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.SeparatorString = "|";
            
            // Speichere mit benutzerdefiniertem Trennzeichen
            workbook.Save("output.txt", txtSaveOptions);
            
            Console.WriteLine("File saved with custom separator successfully.");
        }
    }
}
```

### Siehe auch

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtSaveOptions(SaveFormat) {#constructor_1}

Erstellt Optionen zum Speichern von Textdateien.

```csharp
public TxtSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveFormat | SaveFormat | Das Dateiformat. Es sollte Csv oder Tsv sein, andernfalls wird das gespeicherte Format automatisch auf Csv gesetzt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class TxtSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // Rufen Sie die #ctor-Methode mit dem SaveFormat-Parameter auf
                TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
                
                // Konfigurieren Sie die Speicheroptionen
                saveOptions.Separator = ',';
                saveOptions.Encoding = Encoding.UTF8;
                saveOptions.QuoteType = TxtValueQuoteType.Always;
                
                Console.WriteLine("TxtSaveOptions created successfully with SaveFormat.Csv");
                
                // Speichern Sie die Arbeitsmappe mit den konfigurierten Optionen
                workbook.Save("TxtSaveOptionsDemo.csv", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing TxtSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [SaveFormat](../../saveformat/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


