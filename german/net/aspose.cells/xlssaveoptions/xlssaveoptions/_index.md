---
title: "XlsSaveOptions.XlsSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XlsSaveOptions-Konstruktor. Erstellt Optionen zum Speichern einer Excel 972003 xls-Datei"
type: docs
url: /de/net/aspose.cells/xlssaveoptions/xlssaveoptions/
---
## XlsSaveOptions() {#constructor}

Erstellt Optionen zum Speichern von Excel‑97‑2003‑xls‑Dateien.

```csharp
public XlsSaveOptions()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Sample XLS File");
            worksheet.Cells["A2"].PutValue("Created using XlsSaveOptions");

            // Initialisieren Sie XlsSaveOptions mit dem Konstruktor
            XlsSaveOptions saveOptions = new XlsSaveOptions();

            // Setzen Sie einige Optionen (nicht unterstützte Eigenschaften entfernt)
            saveOptions.IsTemplate = false;

            // Speichern Sie die Arbeitsmappe mit den Optionen
            workbook.Save("output.xls", saveOptions);

            Console.WriteLine("File saved successfully with XlsSaveOptions.");
        }
    }
}
```

### Siehe auch

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsSaveOptions(SaveFormat) {#constructor_1}

Erstellt Optionen zum Speichern von Excel‑97‑2003‑xls/xlt‑Dateien.

```csharp
public XlsSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveFormat | SaveFormat | Das Dateiformat. Es sollte Excel97To2003 oder Xlt sein, andernfalls wird das gespeicherte Format automatisch auf Excel97To2003 gesetzt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123.45);
            
            try
            {
                // Rufen Sie die #ctor-Methode mit dem SaveFormat-Parameter auf
                XlsSaveOptions saveOptions = new XlsSaveOptions(SaveFormat.Excel97To2003);
                
                // Zusätzliche Eigenschaften festlegen
                saveOptions.MatchColor = true;
                saveOptions.WpsCompatibility = false;
                
                Console.WriteLine("XlsSaveOptions constructor executed successfully with SaveFormat parameter");
                
                // Speichere die Arbeitsmappe mit den angegebenen Optionen
                workbook.Save("XlsSaveOptionsCtorDemo.xls", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing XlsSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [SaveFormat](../../saveformat/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


