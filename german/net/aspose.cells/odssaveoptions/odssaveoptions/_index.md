---
title: "OdsSaveOptions.OdsSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsSaveOptions constructor. Erstellt die Optionen zum Speichern einer ODS-Datei"
type: docs
url: /de/net/aspose.cells/odssaveoptions/odssaveoptions/
---
## OdsSaveOptions() {#constructor}

Erstellt die Optionen zum Speichern einer ODS-Datei.

```csharp
public OdsSaveOptions()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispielzellen mit unterschiedlichen Rahmenstilen hinzu
            worksheet.Cells["B2"].PutValue("Medium Border");
            worksheet.Cells["B4"].PutValue("Thick Border");
            worksheet.Cells["B7"].PutValue("Double Border");
            
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Medium;
            worksheet.Cells["B2"].SetStyle(style);
            
            style = workbook.CreateStyle();
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thick;
            worksheet.Cells["B4"].SetStyle(style);
            
            style = workbook.CreateStyle();
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
            worksheet.Cells["B7"].SetStyle(style);

            // Demonstriere den OdsSaveOptions-Konstruktor
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.GeneratorType = Aspose.Cells.Ods.OdsGeneratorType.LibreOffice;
            
            // Als ODS-Datei speichern
            workbook.Save("output.ods", saveOptions);
            
            Console.WriteLine("File saved with OdsSaveOptions constructor demo.");
        }
    }
}
```

### Siehe auch

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsSaveOptions(SaveFormat) {#constructor_1}

Erstellt die Optionen zum Speichern einer ODS-Datei.

```csharp
public OdsSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveFormat | SaveFormat | Das Dateiformat. Es sollte Ods, Ots, Fods oder Sxc sein, andernfalls wird das gespeicherte Format automatisch auf Ods gesetzt. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsSaveOptionsMethodCtorWithSaveFormatDemo
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
                OdsSaveOptions saveOptions = new OdsSaveOptions(SaveFormat.Ods);
                
                // Setzen Sie einige Eigenschaften der Speicheroptionen
                saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
                saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;
                
                Console.WriteLine("OdsSaveOptions constructor executed successfully with SaveFormat.Ods parameter");
                
                // Speichere die Arbeitsmappe mit den angegebenen Optionen
                workbook.Save("OdsSaveOptionsCtorDemo.ods", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing OdsSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [SaveFormat](../../saveformat/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


