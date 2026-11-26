---
title: "Range.CopyValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Copia el valor de la celda de un rango de origen"
type: docs
url: /es/net/aspose.cells/range/copyvalue/
---
## Range.CopyValue method

Copia el valor de la celda de un rango de origen.

```csharp
public void CopyValue(Range range)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | Range | Objeto [`Range`](../) de origen. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyValueWithRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregue una hoja y obtenga la primera hoja
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "SourceSheet";
            
            // Agregar otra hoja de cálculo para el destino
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "DestinationSheet";
            
            // Crear datos de muestra en el rango de origen
            Cells cellsSrc = sheetSrc.Cells;
            cellsSrc["A1"].PutValue("Source Data");
            cellsSrc["A2"].PutValue(10);
            cellsSrc["B2"].PutValue(20);
            cellsSrc["A3"].PutValue(30);
            cellsSrc["B3"].PutValue(40);
            
            // Crear rangos para el origen y el destino
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A2:B3");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("D2:E3");
            
            // Copiar valores del rango de origen al rango de destino
            rangeDest.CopyValue(rangeSrc);
            
            // Guarda el libro de trabajo
            workbook.Save("RangeCopyValueDemo.xlsx");
            
            Console.WriteLine("Values copied successfully from source range to destination range.");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


