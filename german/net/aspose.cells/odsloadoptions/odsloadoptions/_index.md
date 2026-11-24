---
title: "OdsLoadOptions.OdsLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsLoadOptions-Konstruktor. Stellt die Optionen für das Laden einer ODS-Datei dar"
type: docs
url: /de/net/aspose.cells/odsloadoptions/odsloadoptions/
---
## OdsLoadOptions() {#constructor}

Stellt die Optionen für das Laden einer ODS-Datei dar.

```csharp
public OdsLoadOptions()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Erstelle OdsLoadOptions mit dem Konstruktor
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            
            // Setze Hyperlink-Stil, um Excel-Standardwerte zu verwenden
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            
            // Lade ODS-Datei mit den Ladeoptionen
            Workbook workbook = new Workbook("example.ods", loadOptions);
            
            // Als XLSX speichern
            workbook.Save("output.xlsx");
            
            // Überprüfe, ob der Hyperlink-Stil angewendet wurde
            Console.WriteLine("Hyperlink style color: " + 
                workbook.Worksheets[0].Cells["B1"].GetStyle().Font.Color);
        }
    }
}
```

### Siehe auch

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsLoadOptions(LoadFormat) {#constructor_1}

Stellt die Optionen für das Laden einer ODS-Datei dar.

```csharp
public OdsLoadOptions(LoadFormat type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | LoadFormat | Der Ladeformattyp. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class OdsLoadOptionsMethodCtorWithLoadFormatDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispiel-ODS-Datei, falls sie nicht existiert
            string inputFile = "input.ods";
            if (!File.Exists(inputFile))
            {
                using (Workbook sampleWorkbook = new Workbook())
                {
                    sampleWorkbook.Worksheets[0].Hyperlinks.Add("A1", 1, 1, "https://example.com");
                    sampleWorkbook.Save(inputFile, SaveFormat.Ods);
                }
            }

            // Erstelle OdsLoadOptions mit dem LoadFormat-Parameter
            OdsLoadOptions loadOptions = new OdsLoadOptions(LoadFormat.Ods);
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            try
            {
                // Lade Arbeitsmappe mit den erstellten Ladeoptionen
                using (Workbook workbook = new Workbook(inputFile, loadOptions))
                {
                    Console.WriteLine($"Hyperlink style applied: {loadOptions.ApplyExcelDefaultStyleToHyperlink}");
                    
                    // Speichere, um das erfolgreiche Laden zu demonstrieren
                    workbook.Save("OdsLoadOptionsCtorDemo.xlsx");
                }
            }
            catch (FileNotFoundException)
            {
                Console.WriteLine("Error: Created sample file missing - please verify permissions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading ODS file: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [LoadFormat](../../loadformat/)
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


