---
title: "HtmlTableLoadOption.TargetSheetIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlTableLoadOption-egenskap. Hämta eller ange målindexet för kalkylbladet där tabellen ska placeras"
type: docs
url: /sv/net/aspose.cells/htmltableloadoption/targetsheetindex/
---
## HtmlTableLoadOption.TargetSheetIndex property

Hämta eller ange målindexet för kalkylbladet där tabellen ska placeras.

```csharp
public int TargetSheetIndex { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTargetSheetIndexDemo
    {
        public static void Run()
        {
            // Skapa HTML‑laddningsalternativ
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // Konfigurera tabellens laddningsalternativ med TargetSheetIndex
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            tableLoadOption1.TargetSheetIndex = 0; // Load to first worksheet
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1; // Load to second worksheet
            
            // Lägg till tabellens laddningsalternativ
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);
            
            // Läs in HTML-fil med alternativ
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Verifiera att tabellerna har laddats till rätt blad
            Console.WriteLine("Table1 loaded to sheet index: " + tableLoadOption1.TargetSheetIndex);
            Console.WriteLine("Table2 loaded to sheet index: " + tableLoadOption2.TargetSheetIndex);
        }
    }
}
```

### Se även

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


