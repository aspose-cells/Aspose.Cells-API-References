---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions‑konstruktor. Skapar alternativ för att spara html‑fil"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions() {#constructor}

Skapar alternativ för att spara en html‑fil.

```csharp
public HtmlSaveOptions()
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Initiera HtmlSaveOptions med hjälp av konstruktor
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            
            // Spara som HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file saved to: " + outputPath);
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlSaveOptions(SaveFormat) {#constructor_1}

Skapar alternativ för att spara en htm‑fil.

```csharp
public HtmlSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | SaveFormat | Filformatet. Det bör vara någon av följande typer: Html eller MHtml, annars kommer det sparade formatet automatiskt att sättas till Html. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i arbetsbladet
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["C3"].PutValue(DateTime.Now);
            
            try
            {
                // Skapa HtmlSaveOptions med SaveFormat‑parameter
                HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
                
                // Ställ in några egenskaper
                saveOptions.PageTitle = "Aspose.Cells HTML Export";
                saveOptions.ExportActiveWorksheetOnly = true;
                saveOptions.ExportGridLines = true;
                
                // Spara arbetsboken med HtmlSaveOptions
                workbook.Save("HtmlExportWithOptions.html", saveOptions);
                
                Console.WriteLine("HTML file saved successfully with HtmlSaveOptions(SaveFormat)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HtmlSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [SaveFormat](../../saveformat/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


