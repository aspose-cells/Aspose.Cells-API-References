---
title: "Enum NameScopeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.NameScopeType enum. Representerar omfattningstypen för definierade namn"
type: docs
url: /sv/net/aspose.cells/namescopetype/
---
## NameScopeType enumeration

Representerar omfattningstypen för definierade namn.

```csharp
public enum NameScopeType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| All | `0` | Alla definierade namn. |
| Workbook | `1` | De definierade namnen i arbetsboken. |
| Worksheet | `2` | De definierade namnen i ett kalkylblad eller alla kalkylblad. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassNameScopeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            int globalIndex = workbook.Worksheets.Names.Add("GlobalName");
            Name globalName = workbook.Worksheets.Names[globalIndex];
            globalName.RefersTo = "=Sheet1!$A$1";
            
            int index1 = workbook.Worksheets.Names.Add("SheetLevel1");
            Name sheetLevelName1 = workbook.Worksheets.Names[index1];
            sheetLevelName1.RefersTo = "=Sheet1!$A$2";
            sheetLevelName1.SheetIndex = 0;
            
            int index2 = workbook.Worksheets.Names.Add("SheetLevel2");
            Name sheetLevelName2 = workbook.Worksheets.Names[index2];
            sheetLevelName2.RefersTo = "=Sheet2!$A$1";
            sheetLevelName2.SheetIndex = 1;

            Console.WriteLine("Workbook scope names: " + 
                workbook.Worksheets.Names.Filter(NameScopeType.Workbook, -1).Length);
            Console.WriteLine("All worksheet scope names: " + 
                workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1).Length);
            Console.WriteLine("Worksheet scope names (sheet index 0): " + 
                workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 0).Length);
            Console.WriteLine("Worksheet scope names (sheet index 1): " + 
                workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 1).Length);
            Console.WriteLine("All defined names: " + 
                workbook.Worksheets.Names.Filter(NameScopeType.All, -1).Length);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


