---
title: "HtmlLoadOptions.TableLoadOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlLoadOptions egenskap. Hämta HtmlTableLoadOptionCollection-instansen"
type: docs
url: /sv/net/aspose.cells/htmlloadoptions/tableloadoptions/
---
## HtmlLoadOptions.TableLoadOptions property

Hämta HtmlTableLoadOptionCollection‑instansen

```csharp
public HtmlTableLoadOptionCollection TableLoadOptions { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyTableLoadOptionsDemo
    {
        public static void Run()
        {
            // Skapa HTML‑laddningsalternativ
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            
            // Lägg till tabellinläsningsalternativ efter index
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            
            // Lägg till tabellinläsningsalternativ efter ID
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table2";
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Ladda HTML‑fil med alternativen
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Spara utdata
            workbook.Save("output.xlsx");
            
            // Rensa och lägg till nya tabellinläsningsalternativ
            loadOptions.TableLoadOptions.Clear();
            
            // Lägg till tabellinläsningsalternativ med bladindexmappning
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 -> Sheet 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 -> Sheet 0
            
            // Lägg till tabellinläsningsalternativ med ID- och bladmappning
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "mainTable";
            tableLoadOption.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            // Läs in och spara igen med nya alternativ
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output_mapped.xlsx");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOptionCollection](../../htmltableloadoptioncollection/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


