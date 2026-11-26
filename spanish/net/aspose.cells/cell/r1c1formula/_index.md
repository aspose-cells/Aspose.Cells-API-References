---
title: "Cell.R1C1Formula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene o establece una fórmula R1C1 de la celda"
type: docs
url: /es/net/aspose.cells/cell/r1c1formula/
---
## Cell.R1C1Formula property

Obtiene o establece una fórmula R1C1 del [`Cell`](../).

```csharp
public string R1C1Formula { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyR1C1FormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establezca el valor A1
            worksheet.Cells["A1"].PutValue(10);
            
            // Establezca el valor B1
            worksheet.Cells["B1"].PutValue(20);
            
            // Establezca la fórmula C1 en notación A1
            worksheet.Cells["C1"].Formula = "=A1+B1";
            
            // Obtenga y muestre la fórmula R1C1
            string r1c1Formula = worksheet.Cells["C1"].R1C1Formula;
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
            
            // Establezca la fórmula D1 en notación R1C1
            worksheet.Cells["D1"].R1C1Formula = "=RC[-3]+RC[-2]";
            
            // Obtenga y muestre la fórmula A1
            string a1Formula = worksheet.Cells["D1"].Formula;
            Console.WriteLine("A1 Formula: " + a1Formula);
            
            // Guarda el libro de trabajo
            workbook.Save("R1C1FormulaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


