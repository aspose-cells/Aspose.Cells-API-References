---
title: "OoxmlSaveOptions.OoxmlSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OoxmlSaveOptions-konstruktor. Skapar alternativen för att spara Office Open XML-fil"
type: docs
url: /sv/net/aspose.cells/ooxmlsaveoptions/ooxmlsaveoptions/
---
## OoxmlSaveOptions() {#constructor}

Skapar alternativen för att spara Office Open XML‑fil.

```csharp
public OoxmlSaveOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Öppna det första kalkylbladet och lägg till data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Demonstrera OoxmlSaveOptions-konstruktor
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6;
            
            // Spara arbetsboken med OOXML-alternativ
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML options.");
        }
    }
}
```

### Se även

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OoxmlSaveOptions(SaveFormat) {#constructor_1}

Skapar alternativen för att spara Office Open XML‑fil.

```csharp
public OoxmlSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | SaveFormat | Filformatet. Det bör vara en av följande typer: Xlsx, Xltx, Xlam, Xlsm eller Xltm, annars kommer det sparade formatet att automatiskt sättas till Xlsx. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            try
            {
                // Skapa OoxmlSaveOptions med SaveFormat-parameter
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                
                // Ställ in några egenskaper för sparalternativen
                saveOptions.ExportCellName = true;
                saveOptions.CompressionType = OoxmlCompressionType.Level6;
                
                Console.WriteLine("OoxmlSaveOptions created successfully with SaveFormat.Xlsx");
                
                // Spara arbetsboken med de angivna alternativen
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

### Se även

* enum [SaveFormat](../../saveformat/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


