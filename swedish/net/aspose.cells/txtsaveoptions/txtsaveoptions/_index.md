---
title: "TxtSaveOptions.TxtSaveOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtSaveOptions‑konstruktor. Skapar sparalternativ för textfil"
type: docs
url: /sv/net/aspose.cells/txtsaveoptions/txtsaveoptions/
---
## TxtSaveOptions() {#constructor}

Skapar sparalternativ för textfil.

```csharp
public TxtSaveOptions()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            
            // Demonstrera TxtSaveOptions‑konstruktor
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.SeparatorString = "|";
            
            // Spara med anpassad separator
            workbook.Save("output.txt", txtSaveOptions);
            
            Console.WriteLine("File saved with custom separator successfully.");
        }
    }
}
```

### Se även

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## TxtSaveOptions(SaveFormat) {#constructor_1}

Skapar sparalternativ för textfil.

```csharp
public TxtSaveOptions(SaveFormat saveFormat)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | SaveFormat | Filformatet. Det bör vara Csv eller Tsv, annars kommer det sparade formatet att automatiskt sättas till Csv. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class TxtSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            try
            {
                // Anropa #ctor‑metoden med SaveFormat‑parameter
                TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
                
                // Konfigurera sparalternativen
                saveOptions.Separator = ',';
                saveOptions.Encoding = Encoding.UTF8;
                saveOptions.QuoteType = TxtValueQuoteType.Always;
                
                Console.WriteLine("TxtSaveOptions created successfully with SaveFormat.Csv");
                
                // Spara arbetsboken med de konfigurerade alternativen
                workbook.Save("TxtSaveOptionsDemo.csv", saveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing TxtSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [SaveFormat](../../saveformat/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


