---
title: "OoxmlSaveOptions.OoxmlSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OoxmlSaveOptions-Konstruktor. Erstellt die Optionen zum Speichern einer Office-Open-XML-Datei"
type: docs
url: /de/net/aspose.cells/ooxmlsaveoptions/ooxmlsaveoptions/
---
## OoxmlSaveOptions() {#constructor}

Erstellt die Optionen zum Speichern von Office Open XML-Dateien.

```csharp
public OoxmlSaveOptions()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Daten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Demonstrieren Sie den OoxmlSaveOptions-Konstruktor
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6;
            
            // Speichern Sie die Arbeitsmappe mit OOXML-Optionen
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML options.");
        }
    }
}
```

### Siehe auch

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OoxmlSaveOptions(SaveFormat) {#constructor_1}

Erstellt die Optionen zum Speichern von Office Open XML-Dateien.

```csharp
public OoxmlSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveFormat | SaveFormat | Das Dateiformat. Es sollte einer der folgenden Typen entsprechen: Xlsx, Xltx, Xlam, Xlsm oder Xltm, andernfalls wird das gespeicherte Format automatisch auf Xlsx gesetzt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            try
            {
                // Erstellen Sie OoxmlSaveOptions mit dem SaveFormat-Parameter
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                
                // Setzen Sie einige Eigenschaften der Speicheroptionen
                saveOptions.ExportCellName = true;
                saveOptions.CompressionType = OoxmlCompressionType.Level6;
                
                Console.WriteLine("OoxmlSaveOptions created successfully with SaveFormat.Xlsx");
                
                // Speichere die Arbeitsmappe mit den angegebenen Optionen
                workbook.Save("OoxmlSaveOptionsCtorDemo.xlsx", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating OoxmlSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [SaveFormat](../../saveformat/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


