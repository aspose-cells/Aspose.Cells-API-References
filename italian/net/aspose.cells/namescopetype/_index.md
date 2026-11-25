---
title: "Enum NameScopeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.NameScopeType. Rappresenta il tipo di ambito dei nomi definiti"
type: docs
url: /it/net/aspose.cells/namescopetype/
---
## NameScopeType enumeration

Rappresenta il tipo di ambito dei nomi definiti.

```csharp
public enum NameScopeType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| All | `0` | Tutti i nomi definiti. |
| Workbook | `1` | I nomi definiti nella cartella di lavoro. |
| Worksheet | `2` | I nomi definiti in un foglio di lavoro o in tutti i fogli. |

### Esempi

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

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


