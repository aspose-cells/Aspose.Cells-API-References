---
title: "Cell.IsTableFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Indica si esta celda es parte de la fórmula de tabla"
type: docs
url: /es/net/aspose.cells/cell/istableformula/
---
## Cell.IsTableFormula property

Indica si esta celda forma parte de una fórmula de tabla.

```csharp
public bool IsTableFormula { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellPropertyIsTableFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear una tabla
            int index = worksheet.ListObjects.Add(0, 0, 5, 3, true);
            ListObject table = worksheet.ListObjects[index];
            
            // Agregar fórmula de tabla a la celda D2
            Cell cell = worksheet.Cells["D2"];
            cell.Formula = "=SUM(Table1[[#This Row],[Column1]:[Column3]])";
            
            // Comprobar si la celda contiene una fórmula de tabla
            Console.WriteLine("Is table formula: " + cell.IsTableFormula);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


