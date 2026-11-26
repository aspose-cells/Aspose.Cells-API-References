---
title: "Range.CopyData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Copia datos de celdas incluyendo fórmulas de un rango de origen"
type: docs
url: /es/net/aspose.cells/range/copydata/
---
## Range.CopyData method

Copia datos de celda (incluidas fórmulas) de un rango de origen.

```csharp
public void CopyData(Range range)
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
    public class RangeMethodCopyDataWithRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtén la primera worksheet y agrega algunos datos
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            sheetSrc.Cells["A1"].PutValue("Source Data");
            sheetSrc.Cells["B1"].PutValue(100);
            sheetSrc.Cells["A2"].PutValue("More Data");
            sheetSrc.Cells["B2"].PutValue(200);

            // Agrega una worksheet de destino
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";

            // Crea rangos de origen y de destino
            Aspose.Cells.Range rangeSrc = sheetSrc.Cells.CreateRange("A1:B2");
            Aspose.Cells.Range rangeDest = sheetDest.Cells.CreateRange("C3:D4");

            // Copia datos del rango de origen al rango de destino
            rangeDest.CopyData(rangeSrc);

            // Guarda el libro de trabajo
            workbook.Save("RangeCopyDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


