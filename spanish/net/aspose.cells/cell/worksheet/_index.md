---
title: "Cell.Worksheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene la hoja de cálculo principal"
type: docs
url: /es/net/aspose.cells/cell/worksheet/
---
## Cell.Worksheet property

Obtiene la hoja de cálculo principal.

```csharp
public Worksheet Worksheet { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
            
            // Acceder a una celda y demostrar la propiedad Worksheet
            Cell cell = worksheet.Cells["A3"];
            
            // Mostrar información de la hoja de cálculo a través de la propiedad Worksheet de la celda
            Console.WriteLine("Cell A3 is in worksheet: " + cell.Worksheet.Name);
            Console.WriteLine("Calculation result in A3: " + cell.Value);
            
            // Agregar otra hoja de cálculo y demostrar la referencia cruzada de hoja
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["B1"].PutValue("=A3");
            
            // Acceder a la celda en Sheet2 y mostrar su hoja de cálculo
            Cell crossSheetCell = sheet2.Cells["B1"];
            Console.WriteLine("Cell B1 is in worksheet: " + crossSheetCell.Worksheet.Name);
            Console.WriteLine("Cross-sheet reference in B1: " + crossSheetCell.Value);
        }
    }
}
```

### Ver también

* class [Worksheet](../../worksheet/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


