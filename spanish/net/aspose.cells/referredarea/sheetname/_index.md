---
title: "ReferredArea.SheetName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ReferredArea. Indica en qué hoja está esta referencia"
type: docs
url: /es/net/aspose.cells/referredarea/sheetname/
---
## ReferredArea.SheetName property

Indica en qué hoja se encuentra esta referencia.

```csharp
public string SheetName { get; }
```

### Observaciones

Si hace referencia a varias hojas de cálculo, el valor devuelto es como la expresión de rango en la fórmula. Por ejemplo "Sheet1:Sheet3" para la referencia en la fórmula "=SUM(Sheet1:Sheet3!$A$1:$B$2)".

### Ejemplos

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

### Ver también

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


