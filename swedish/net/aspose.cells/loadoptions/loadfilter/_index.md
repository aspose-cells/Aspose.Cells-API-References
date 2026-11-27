---
title: "LoadOptions.LoadFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions‑egenskap. Filtret som anger hur data ska läsas in"
type: docs
url: /sv/net/aspose.cells/loadoptions/loadfilter/
---
## LoadOptions.LoadFilter property

Filtret som anger hur data ska laddas.

```csharp
public LoadFilter LoadFilter { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomLoadFilter : LoadFilter
    {
        public override void StartSheet(Worksheet sheet)
        {
            // Läs endast in data om bladet är synligt
            if (sheet.IsVisible)
            {
                base.StartSheet(sheet);
            }
        }
    }

    public class LoadOptionsPropertyLoadFilterDemo
    {
        public static void Run()
        {
            // Skapa en testarbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "HiddenSheet";
            sheet.IsVisible = false;
            sheet.Cells["A1"].PutValue("This should not load");
            
            // Lägg till ett synligt blad
            Worksheet visibleSheet = workbook.Worksheets.Add("VisibleSheet");
            visibleSheet.Cells["A1"].PutValue("This will load");
            
            // Spara testfilen
            string filePath = "LoadFilterTest.xlsx";
            workbook.Save(filePath);
            workbook.Dispose();

            // Läs in med anpassat filter
            LoadOptions options = new LoadOptions();
            options.LoadFilter = new CustomLoadFilter();
            
            Workbook loadedWorkbook = new Workbook(filePath, options);
            
            // Verifiera att endast det synliga bladet har lästs in
            Console.WriteLine("Loaded Sheets:");
            foreach (Worksheet ws in loadedWorkbook.Worksheets)
            {
                Console.WriteLine($"- {ws.Name}: Visible={ws.IsVisible}");
                if (ws.IsVisible)
                {
                    Console.WriteLine($"  A1 Value: {ws.Cells["A1"].StringValue}");
                }
            }
            
            loadedWorkbook.Dispose();
        }
    }
}
```

### Se även

* class [LoadFilter](../../loadfilter/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


