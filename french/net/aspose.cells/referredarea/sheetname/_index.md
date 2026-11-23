---
title: "ReferredArea.SheetName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ReferredArea. Indique dans quelle feuille cette référence se trouve"
type: docs
url: /fr/net/aspose.cells/referredarea/sheetname/
---
## ReferredArea.SheetName property

Indique dans quelle feuille se trouve cette référence.

```csharp
public string SheetName { get; }
```

### Remarques

Si elle fait référence à plusieurs feuilles de calcul, la valeur retournée est similaire à l'expression de plage dans la formule. Par exemple "Sheet1:Sheet3" pour la référence dans la formule "=SUM(Sheet1:Sheet3!$A$1:$B$2)".

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertySheetNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            Worksheet worksheet1 = workbook.Worksheets["Sheet1"];
            
            workbook.Worksheets["Sheet2"].Cells.CreateRange("E5:I6").Name = "someNamedRange_1";
            worksheet1.Cells["A1"].Formula = "=SUM(someNamedRange_1)";
            
            ReferredArea ra = worksheet1.Cells["A1"].GetPrecedents()[0];
            Console.WriteLine("Precedent's referred sheet: " + ra.SheetName);
        }
    }
}
```

### Voir aussi

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


