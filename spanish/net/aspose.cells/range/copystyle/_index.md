---
title: "Range.CopyStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Copia la configuración de estilo de un rango origen"
type: docs
url: /es/net/aspose.cells/range/copystyle/
---
## Range.CopyStyle method

Copia la configuración de estilo de un rango de origen.

```csharp
public void CopyStyle(Range range)
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
    public class RangeMethodCopyStyleWithRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            
            // Agregar un estilo de ejemplo al rango origen
            Cells cellsSrc = sheetSrc.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A1:D5");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            rangeSrc.SetStyle(style);
            
            // Crear hoja de cálculo de destino
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";
            
            // Crear rango de destino y copiar estilo
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange("A1:D5");
            rangeDest.CopyStyle(rangeSrc);
            
            // Guarda el libro de trabajo
            workbook.Save("RangeCopyStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


