---
title: "SaveOptions.CheckExcelRestriction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SaveOptions-egenskap. Anger om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter inte Excel att ange en strängvärde längre än 32 K. När du anger ett värde längre än 32 K kommer det att trunkeras"
type: docs
url: /sv/net/aspose.cells/saveoptions/checkexcelrestriction/
---
## SaveOptions.CheckExcelRestriction property

Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32K. När du matar in ett värde längre än 32K kommer det att trunkeras.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Inaktivera kontroll av Excel-restriktioner
            workbook.Settings.CheckExcelRestriction = false;

            // Åtkomst till första arbetsbladet och cellerna
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Skapa en sträng som är längre än Excels normala gräns
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // Placera den långa strängen i cell A1
            cells["A1"].PutValue(longString);

            // Konfigurera sparaalternativ för att kringgå begränsningar
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;

            // Spara arbetsboken
            workbook.Save("output_without_restrictions.xlsx", saveOptions);

            // Läs in den sparade filen med begränsningar inaktiverade
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output_without_restrictions.xlsx", loadOptions);

            // Verifiera att den långa strängen bevarades
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("Loaded string length: " + loadedValue.Length);
            Console.WriteLine("First 50 chars: " + loadedValue.Substring(0, 50));
            Console.WriteLine("Last 50 chars: " + loadedValue.Substring(loadedValue.Length - 50));
        }
    }
}
```

### Se även

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


