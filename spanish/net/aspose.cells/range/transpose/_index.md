---
title: "Range.Transpose"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Transponer rota los datos de filas a columnas o viceversa"
type: docs
url: /es/net/aspose.cells/range/transpose/
---
## Range.Transpose method

Transponer (rotar) datos de filas a columnas o viceversa.

```csharp
public void Transpose()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodTransposeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Llena datos de muestra en un rango de 3x3 (A1:C3)
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].PutValue(6);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["C3"].PutValue(9);
            
            // Crea un rango (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            
            // Transponer el rango
            range.Transpose();
            
            // Guarda el libro de trabajo
            workbook.Save("TransposedOutput.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


