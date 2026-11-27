---
title: "LoadOptions.CheckExcelRestriction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions‑egenskap. Anger om restriktioner för Excel‑filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att mata in en strängvärde längre än 32 K. När du matar in ett värde längre än 32 K, t.ex. via Cell.PutValuestring, får du ett Exception om denna egenskap är true. Om egenskapen är false accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan skriva ut hela strängvärdet för andra filformat som CSV. Men om du har angett ett värde som är ogiltigt för Excel‑filformatet bör du inte spara arbetsboken som Excel‑filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel‑filen."
type: docs
url: /sv/net/aspose.cells/loadoptions/checkexcelrestriction/
---
## LoadOptions.CheckExcelRestriction property

Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att en strängvärde längre än 32 K matas in. När du matar in ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett undantag om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan exportera hela strängvärdet till andra filformat som CSV. Däremot, om du har angett ett värde som är ogiltigt för Excel-filformatet bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Inaktivera kontroll av Excel‑restriktioner
            workbook.Settings.CheckExcelRestriction = false;

            // Åtkomst till första arbetsbladet och cellerna
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Skapa en sträng som är längre än Excels normala gräns (32767 tecken)
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // Placera den långa strängen i cell A1
            cells["A1"].PutValue(longString);
            
            // Spara med kontroll av restriktioner inaktiverad
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;
            workbook.Save("output.xlsx", saveOptions);
            
            // Läs in med kontroll av restriktioner inaktiverad
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output.xlsx", loadOptions);
            
            // Verifiera att den långa strängen bevarades
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("String length: " + loadedValue.Length);
            Console.WriteLine("String matches: " + loadedValue.Equals(longString));
        }
    }
}
```

### Se även

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


