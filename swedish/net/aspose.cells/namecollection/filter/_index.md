---
title: "NameCollection.Filter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NameCollection metod. Hämtar alla definierade namn efter omfattning"
type: docs
url: /sv/net/aspose.cells/namecollection/filter/
---
## NameCollection.Filter method

Hämtar alla definierade namn efter omfång.

```csharp
public Name[] Filter(NameScopeType type, int sheetIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | NameScopeType | Omfattningstypen. |
| sheetIndex | Int32 | Bladindexet. Påverkar endast när omfattningstypen är Worksheet |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodFilterWithNameScopeTypeInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till några namn i arbetsboken och kalkylbladen
            workbook.Worksheets.Names.Add("GlobalName");
            Worksheet worksheet1 = workbook.Worksheets[0];
            workbook.Worksheets.Names.Add("Sheet1Name");
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Names.Add("Sheet2Name");

            // Filtrera namn efter omfattningstyp och bladindex
            Name[] workbookScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Workbook, -1);
            Name[] worksheetScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1);
            Name[] sheet1Names = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 0);

            // Skriv ut resultat
            Console.WriteLine($"Workbook-scoped names count: {workbookScopeNames.Length}");
            Console.WriteLine($"Worksheet-scoped names count: {worksheetScopeNames.Length}");
            Console.WriteLine($"Sheet1 names count: {sheet1Names.Length}");
        }
    }
}
```

### Se även

* class [Name](../../name/)
* enum [NameScopeType](../../namescopetype/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


