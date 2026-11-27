---
title: "LowCodeSplitOptions.SaveOptionsProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSplitOptions‑egenskap. Leverantör av sparalternativ för att spara de delade delarna"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/
---
## LowCodeSplitOptions.SaveOptionsProvider property

Leverantör av sparaalternativ för att spara de delade delarna.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Anmärkningar

Om den här egenskapen anges, [`SaveOptions`](../saveoptions/) har ingen effekt eftersom utdata för varje delad del kommer att anges av leverantören.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fyll i lite exempeldata
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // Skapa en LowCodeSplitOptions‑instans
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // Visa aktuellt SaveOptionsProvider‑värde (null som standard)
            Console.WriteLine("Current SaveOptionsProvider value: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Skapa en anpassad SaveOptionsProvider
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // Demonstrera effekten av att sätta SaveOptionsProvider
            // I ett verkligt scenario skulle detta användas vid delning av filer
            Console.WriteLine("After setting SaveOptionsProvider: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Spara arbetsboken (även om delning inte demonstreras här)
            workbook.Save("PropertySaveOptionsProviderDemo.xlsx");
        }
    }

    // Anpassad implementation av AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Skapa anpassade sparalternativ för varje delad del
            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            return options;
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Utför eventuell städning efter att varje del har sparats
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### Se även

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


