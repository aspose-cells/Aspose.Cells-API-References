---
title: "OdsLoadOptions.OdsLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsLoadOptions konstruktor. Representerar alternativen för att läsa in ods-fil"
type: docs
url: /sv/net/aspose.cells/odsloadoptions/odsloadoptions/
---
## OdsLoadOptions() {#constructor}

Representerar alternativen för att läsa in ods-fil.

```csharp
public OdsLoadOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa OdsLoadOptions med hjälp av konstruktorn
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            
            // Ange hyperlänkstil för att använda Excels standardinställningar
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;
            
            // Läs in ODS-fil med laddningsalternativen
            Workbook workbook = new Workbook("example.ods", loadOptions);
            
            // Spara som XLSX
            workbook.Save("output.xlsx");
            
            // Verifiera att hyperlänkstilen har tillämpats
            Console.WriteLine("Hyperlink style color: " + 
                workbook.Worksheets[0].Cells["B1"].GetStyle().Font.Color);
        }
    }
}
```

### Se även

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsLoadOptions(LoadFormat) {#constructor_1}

Representerar alternativen för att läsa in ods-fil.

```csharp
public OdsLoadOptions(LoadFormat type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | LoadFormat | Inläsningsformatstypen. |

### Exempel

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
            // Skapa ett exempel på ODS-fil om den inte finns
            string inputFile = "input.ods";
            if (!File.Exists(inputFile))
            {
                using (Workbook sampleWorkbook = new Workbook())
                {
                    sampleWorkbook.Worksheets[0].Hyperlinks.Add("A1", 1, 1, "https://example.com");
                    sampleWorkbook.Save(inputFile, SaveFormat.Ods);
                }
            }

            // Skapa OdsLoadOptions med LoadFormat-parameter
            OdsLoadOptions loadOptions = new OdsLoadOptions(LoadFormat.Ods);
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            try
            {
                // Läs in arbetsbok med skapade laddningsalternativ
                using (Workbook workbook = new Workbook(inputFile, loadOptions))
                {
                    Console.WriteLine($"Hyperlink style applied: {loadOptions.ApplyExcelDefaultStyleToHyperlink}");
                    
                    // Spara för att demonstrera lyckad inläsning
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

### Se även

* enum [LoadFormat](../../loadformat/)
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


