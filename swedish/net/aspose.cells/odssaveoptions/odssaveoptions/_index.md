---
title: "OdsSaveOptions.OdsSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsSaveOptions‑konstruktorn. Skapar alternativen för att spara ods‑fil"
type: docs
url: /sv/net/aspose.cells/odssaveoptions/odssaveoptions/
---
## OdsSaveOptions() {#constructor}

Skapar alternativen för att spara ods‑fil.

```csharp
public OdsSaveOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempelceller med olika kantstilar
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

            // Demonstrera OdsSaveOptions‑konstruktorn
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.GeneratorType = Aspose.Cells.Ods.OdsGeneratorType.LibreOffice;
            
            // Spara som ODS‑fil
            workbook.Save("output.ods", saveOptions);
            
            Console.WriteLine("File saved with OdsSaveOptions constructor demo.");
        }
    }
}
```

### Se även

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## OdsSaveOptions(SaveFormat) {#constructor_1}

Skapar alternativen för att spara ods‑fil.

```csharp
public OdsSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | SaveFormat | Filformatet. Det bör vara Ods, Ots, Fods eller Sxc, annars kommer det sparade formatet att automatiskt sättas till Ods. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123.45);
            
            try
            {
                // Anropa #ctor‑metoden med SaveFormat‑parameter
                OdsSaveOptions saveOptions = new OdsSaveOptions(SaveFormat.Ods);
                
                // Ställ in några egenskaper för sparalternativen
                saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
                saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;
                
                Console.WriteLine("OdsSaveOptions constructor executed successfully with SaveFormat.Ods parameter");
                
                // Spara arbetsboken med de angivna alternativen
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

### Se även

* enum [SaveFormat](../../saveformat/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


