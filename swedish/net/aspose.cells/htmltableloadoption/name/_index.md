---
title: "HtmlTableLoadOption.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlTableLoadOption-egenskap. Hämta eller ange namnet på tabellen som ska importeras från HTML"
type: docs
url: /sv/net/aspose.cells/htmltableloadoption/name/
---
## HtmlTableLoadOption.Name property

Hämta eller ange namnet på tabellen som ska importeras från HTML

```csharp
[Obsolete("Please use HtmlTableLoadOption.Id instead")]
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Åtkomst till HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Lägg till ett nytt HtmlTableLoadOption med tabellindex
            int index = tableLoadOptions.Add(0);

            // Åtkomst till HtmlTableLoadOption
            HtmlTableLoadOption option = tableLoadOptions[index];

            // Ange Name-egenskapen
            option.Name = "CustomerDataTable";

            // Läs in en HTML-fil (ersätt med faktisk filsökväg)
            workbook = new Workbook("input.html", loadOptions);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


