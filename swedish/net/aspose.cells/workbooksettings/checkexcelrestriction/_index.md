---
title: "WorkbookSettings.CheckExcelRestriction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings property. Anger om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter inte Excel att mata in en strängvärde längre än 32K. När du matar in ett värde längre än 32K, exempelvis via Cell.PutValuestring, får du ett undantag om denna egenskap är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan skriva ut hela strängvärdet för andra filformat som CSV. Om du däremot har angett ett värde som är ogiltigt för Excel-filformatet bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen."
type: docs
url: /sv/net/aspose.cells/workbooksettings/checkexcelrestriction/
---
## WorkbookSettings.CheckExcelRestriction property

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
    public class WorkbookSettingsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Inaktivera kontroll av Excel-restriktioner
            workbook.Settings.CheckExcelRestriction = false;
            
            // Infoga en sträng som överskrider normala Excel-gränser
            string longString = new string('a', 40000);
            workbook.Worksheets[0].Cells["A1"].PutValue(longString);
            
            // Spara och ladda om för att verifiera att restriktionen har kringgåtts
            string tempFile = Guid.NewGuid().ToString() + ".txt";
            workbook.Save(tempFile, new TxtSaveOptions());
            
            Workbook loadedWorkbook = new Workbook(tempFile, new LoadOptions { CheckExcelRestriction = false });
            Console.WriteLine("String length: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue.Length);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


