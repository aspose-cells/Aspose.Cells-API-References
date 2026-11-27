---
title: "HtmlTableLoadOption.Id"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlTableLoadOption-egenskap. Hämta eller ange ID för tabellen som ska importeras från HTML"
type: docs
url: /sv/net/aspose.cells/htmltableloadoption/id/
---
## HtmlTableLoadOption.Id property

Hämta eller ange id för tabellen som ska importeras från HTML

```csharp
public string Id { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyIdDemo
    {
        public static void Run()
        {
            // Skapa HTML‑laddningsalternativ
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Konfigurera tabellens laddningsalternativ
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1"; // Setting Id property
            tableLoadOption1.TargetSheetIndex = 0;
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2"; // Setting Id property
            tableLoadOption2.TargetSheetIndex = 0;

            // Lägg till tabellens laddningsalternativ
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // Läs in HTML-fil med angivna alternativ
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            Console.WriteLine("HTML tables with specified IDs have been loaded to Excel.");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


