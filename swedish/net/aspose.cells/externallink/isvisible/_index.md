---
title: "ExternalLink.IsVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalLink egenskap. Anger om denna externa länk är synlig i MS Excel"
type: docs
url: /sv/net/aspose.cells/externallink/isvisible/
---
## ExternalLink.IsVisible property

Indikerar om denna externa länk är synlig i MS Excel.

```csharp
public bool IsVisible { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med externa länkar
            Workbook workbook = new Workbook();
            
            // Lägg till lite data i det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("External Link Demo");
            
            // Skapa en ny arbetsbok att använda som källa för extern länk
            Workbook externalWorkbook = new Workbook();
            externalWorkbook.Worksheets[0].Cells["A1"].PutValue(100);
            externalWorkbook.Save("external_data.xlsx");
            
            // Lägg till en referens för extern länk
            workbook.Worksheets[0].Cells["B1"].Formula = "='[external_data.xlsx]Sheet1'!A1";
            
            // Kontrollera externa länkar (de kommer att skapas automatiskt när formler laddas)
            foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link visibility: {link.IsVisible}");
                Console.WriteLine($"External link data source: {link.DataSource}");
            }
            
            // Skapa en annan arbetsbok för att demonstrera inläsning av befintlig fil
            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("=SUM([example.xls]Sheet1!A1:A10)");
            
            // Spara och ladda om för att demonstrera externa länkar
            workbook2.Save("output.xlsx");
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Kontrollera externa länkar i den inlästa arbetsboken
            foreach (ExternalLink link in loadedWorkbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link URL: {link.DataSource}, Visible: {link.IsVisible}");
            }
        }
    }
}
```

### Se även

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


