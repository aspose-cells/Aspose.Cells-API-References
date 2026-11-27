---
title: "CalculationOptions.LinkedDataSources"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationOptions-egenskap. Anger datakällorna för externa länkar som används i formler"
type: docs
url: /sv/net/aspose.cells/calculationoptions/linkeddatasources/
---
## CalculationOptions.LinkedDataSources property

Anger datakällorna för externa länkar som används i formler.

```csharp
public Workbook[] LinkedDataSources { get; set; }
```

### Anmärkningar

Som [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/), kan du här ange datakällor för externa länkar som används i formler som ska beräknas, särskilt de som används i INDIRECT-funktionen. För de externa länkar som används i INDIRECT-funktionen tas de inte med som en del av arbetsbokens externa länkar och kan inte uppdateras av [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/). Matchningen av dessa arbetsböcker med externa länkar bestäms av [`FileName`](../../workbook/filename/) och [`DataSource`](../../externallink/datasource/). Så se till att [`FileName`](../../workbook/filename/) har angetts med rätt värde (vanligtvis bör det vara samma som motsvarande [`DataSource`](../../externallink/datasource/)) för varje arbetsbok så att de kan länkas som förväntat.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyLinkedDataSourcesDemo
    {
        public static void Run()
        {
            // Skapa extern arbetsbok med data
            Workbook wbExt = new Workbook();
            wbExt.Worksheets[0].Cells["A2"].PutValue(100);
            wbExt.Worksheets.Add("Sheet2").Cells["A2"].PutValue(200);
            
            // Lägg till namngivna områden i extern arbetsbok
            int nameIndex1 = wbExt.Worksheets.Names.Add("Sheet1!ExtNamedRange1");
            wbExt.Worksheets.Names[nameIndex1].RefersTo = "=Sheet1!$A$2";
            int nameIndex2 = wbExt.Worksheets.Names.Add("Sheet2!ExtNamedRange2");
            wbExt.Worksheets.Names[nameIndex2].RefersTo = "=Sheet2!$A$2";
            int nameIndex3 = wbExt.Worksheets.Names.Add("GlobalNamedRange");
            wbExt.Worksheets.Names[nameIndex3].RefersTo = "=Sheet1!$A$2";

            // Skapa huvudarbetsbok
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ställ in formler som refererar till extern arbetsbok
            sheet.Cells["A1"].Formula = "=[External.xlsx]Sheet1!$A$2";
            sheet.Cells["A2"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!$A$2\")";
            sheet.Cells["A3"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!ExtNamedRange1\")";
            sheet.Cells["A4"].Formula = "=INDIRECT(\"[External.xlsx]!GlobalNamedRange\")";

            // Beräkna formler med hjälp av LinkedDataSources
            CalculationOptions options = new CalculationOptions();
            options.LinkedDataSources = new Workbook[] { wbExt };
            
            Console.WriteLine("Before calculation:");
            PrintCellValues(sheet);

            wb.CalculateFormula(options);
            
            Console.WriteLine("\nAfter calculation:");
            PrintCellValues(sheet);
        }

        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {sheet.Cells[$"A{i+1}"].StringValue}");
            }
        }
    }
}
```

### Se även

* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


