---
title: "WorkbookSettings.PaperSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Hämtar och anger standardpappersstorleken för utskrift"
type: docs
url: /sv/net/aspose.cells/workbooksettings/papersize/
---
## WorkbookSettings.PaperSize property

Hämtar och anger standardpappersstorleken för utskrift.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Anmärkningar

Om det inte finns någon inställning för pappersstorlek, kommer MS Excel att använda standardinställningen för skrivaren.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ställ in pappersstorlek till A5
            workbook.Settings.PaperSize = PaperSizeType.PaperA5;
            
            // Verifiera att pappersstorleken är korrekt inställd i det första kalkylbladet
            Console.WriteLine("Paper size: " + workbook.Worksheets[0].PageSetup.PaperSize);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [PaperSizeType](../../papersizetype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


