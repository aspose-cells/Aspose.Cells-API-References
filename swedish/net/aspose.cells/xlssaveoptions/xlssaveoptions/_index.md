---
title: "XlsSaveOptions.XlsSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XlsSaveOptions‑konstruktor. Skapar alternativ för att spara Excel 972003 xls‑fil"
type: docs
url: /sv/net/aspose.cells/xlssaveoptions/xlssaveoptions/
---
## XlsSaveOptions() {#constructor}

Skapar alternativ för att spara Excel 97‑2003 xls‑fil.

```csharp
public XlsSaveOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Sample XLS File");
            worksheet.Cells["A2"].PutValue("Created using XlsSaveOptions");

            // Initiera XlsSaveOptions med hjälp av konstruktorn
            XlsSaveOptions saveOptions = new XlsSaveOptions();

            // Ställ in några alternativ (borttagna ej stödda egenskaper)
            saveOptions.IsTemplate = false;

            // Spara arbetsboken med alternativen
            workbook.Save("output.xls", saveOptions);

            Console.WriteLine("File saved successfully with XlsSaveOptions.");
        }
    }
}
```

### Se även

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## XlsSaveOptions(SaveFormat) {#constructor_1}

Skapar alternativ för att spara Excel 97‑2003 xls/xlt‑fil.

```csharp
public XlsSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | SaveFormat | Filformatet. Det bör vara Excel97To2003 eller Xlt, annars kommer det sparade formatet automatiskt att sättas till Excel97To2003. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XlsSaveOptionsMethodCtorWithSaveFormatDemo
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
                XlsSaveOptions saveOptions = new XlsSaveOptions(SaveFormat.Excel97To2003);
                
                // Ange ytterligare egenskaper
                saveOptions.MatchColor = true;
                saveOptions.WpsCompatibility = false;
                
                Console.WriteLine("XlsSaveOptions constructor executed successfully with SaveFormat parameter");
                
                // Spara arbetsboken med de angivna alternativen
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

### Se även

* enum [SaveFormat](../../saveformat/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


