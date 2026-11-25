---
title: "Name.SheetIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Name. Indica che questo nome appartiene a Workbook o Worksheet. 0  Nome globale altrimenti indice al foglio basato su 1"
type: docs
url: /it/net/aspose.cells/name/sheetindex/
---
## Name.SheetIndex property

Indica a quale cartella di lavoro o foglio appartiene questo nome. 0 = Nome globale, altrimenti indice al foglio (basato su 1).

```csharp
public int SheetIndex { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertySheetIndexDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni fogli di lavoro
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Crea un intervallo denominato in Sheet2
            Worksheet sheet2 = workbook.Worksheets["Sheet2"];
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet2!$A$1:$B$10";
            
            // Visualizza l'indice del foglio dell'intervallo denominato
            Console.WriteLine("Sheet index of named range: " + name.SheetIndex);
            
            // Salva la cartella di lavoro
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


