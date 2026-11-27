---
title: "PclSaveOptions.AddPrinterFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PclSaveOptions-metoden. Lägger till information om teckensnitt som redan har lagts till i skrivaren av tillverkaren"
type: docs
url: /sv/net/aspose.cells/pclsaveoptions/addprinterfont/
---
## PclSaveOptions.AddPrinterFont method

Lägger till information om teckensnitt som redan har lagts till skrivaren av tillverkaren.

```csharp
public void AddPrinterFont(string fontFullName, string fontPclName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontFullName | String | Fullständigt namn på teckensnittet (t.ex. "Times New Roman Bold Italic") som används i källfilen. |
| fontPclName | String | Namn på teckensnittet som kommer att användas i den utgående Pcl-dokumentet. |

### Anmärkningar

Det finns 52 teckensnitt som ska vara inbyggda i alla skrivare enligt Pcl-specifikationen. Tillverkare kan dock lägga till andra teckensnitt i sina enheter.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodAddPrinterFontWithStringStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite text i kalkylbladet för att demonstrera teckensnittsanvändning.
            worksheet.Cells["A1"].PutValue("This text will use the added printer font");
            
            // Skapa PCL‑spara‑alternativ
            PclSaveOptions pclSaveOptions = new PclSaveOptions();
            
            try
            {
                // Anropa AddPrinterFont-metoden med specifika teckensnittsnamn.
                pclSaveOptions.AddPrinterFont("Arial", "ArialPCL");
                pclSaveOptions.AddPrinterFont("Times New Roman", "TimesPCL");
                
                Console.WriteLine("AddPrinterFont method executed successfully with parameters (String, String)");
                
                // Spara arbetsboken med PCL-alternativ.
                workbook.Save("PclWithAddedPrinterFonts.pcl", pclSaveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPrinterFont method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


