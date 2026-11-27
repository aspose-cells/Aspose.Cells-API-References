---
title: "EbookSaveOptions.EbookSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "EbookSaveOptions‑konstruktor. Skapar alternativ för att spara e-bokfil"
type: docs
url: /sv/net/aspose.cells.saving/ebooksaveoptions/ebooksaveoptions/
---
## EbookSaveOptions() {#constructor}

Skapar alternativ för att spara e‑bokfil.

```csharp
public EbookSaveOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class EbookSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempelinnehåll
            worksheet.Cells["A1"].PutValue("Ebook Test");
            worksheet.Cells["A2"].PutValue("This is a test for EbookSaveOptions");
            
            // Skapa EbookSaveOptions med hjälp av konstruktorn
            EbookSaveOptions saveOptions = new EbookSaveOptions();
            
            // Spara arbetsboken med EbookSaveOptions (sparar automatiskt som EPUB)
            workbook.Save("output.epub", saveOptions);
            
            Console.WriteLine("Ebook saved successfully with EbookSaveOptions constructor.");
        }
    }
}
```

### Se även

* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)

---

## EbookSaveOptions(SaveFormat) {#constructor_1}

Skapar alternativ för att spara e‑bokfil.

```csharp
public EbookSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | SaveFormat | Filformatet. Det bör vara Epub eller Azw3. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class EbookSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i arbetsbladet
            worksheet.Cells["A1"].PutValue("Sample Ebook Content");
            
            try
            {
                // Anropa #ctor‑metoden med SaveFormat‑parameter
                EbookSaveOptions saveOptions = new EbookSaveOptions(SaveFormat.Epub);
                
                // Ange ytterligare egenskaper om det behövs
                saveOptions.Encoding = System.Text.Encoding.UTF8;
                
                Console.WriteLine("EbookSaveOptions constructor executed successfully with SaveFormat.Epub");
                
                // Spara arbetsboken med de skapade alternativen
                workbook.Save("EbookSaveOptionsDemo.epub", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EbookSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [EbookSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


