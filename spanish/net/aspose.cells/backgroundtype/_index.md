---
title: "Enumeración BackgroundType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.BackgroundType. Enumera los tipos de patrones de fondo de celda"
type: docs
url: /es/net/aspose.cells/backgroundtype/
---
## BackgroundType enumeration

Enumera los tipos de patrones de fondo de celda.

```csharp
public enum BackgroundType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DiagonalCrosshatch | `9` | Representa un patrón de cruzado diagonal. |
| DiagonalStripe | `8` | Representa un patrón de rayas diagonal. |
| Gray6 | `18` | Representa un patrón gris del 6,25% |
| Gray12 | `17` | Representa un patrón gris del 12,5% |
| Gray25 | `4` | Representa un patrón gris del 25%. |
| Gray50 | `2` | Representa un patrón gris del 50%. |
| Gray75 | `3` | Representa un patrón gris del 75%. |
| HorizontalStripe | `5` | Representa un patrón de rayas horizontal. |
| None | `0` | Representa sin fondo. |
| ReverseDiagonalStripe | `7` | Representa un patrón de rayas diagonal inversa. |
| Solid | `1` | Representa un patrón sólido. |
| ThickDiagonalCrosshatch | `10` | Representa un patrón de cruzado diagonal grueso. |
| ThinDiagonalCrosshatch | `16` | Representa un patrón de cruzado diagonal delgado. |
| ThinDiagonalStripe | `14` | Representa un patrón de rayas diagonal delgado. |
| ThinHorizontalCrosshatch | `15` | Representa un patrón de cruzado horizontal delgado. |
| ThinHorizontalStripe | `11` | Representa un patrón de rayas horizontal delgado. |
| ThinReverseDiagonalStripe | `13` | Representa un patrón de rayas diagonal inversa delgado. |
| ThinVerticalStripe | `12` | Representa un patrón de franjas verticales delgadas. |
| VerticalStripe | `6` | Representa un patrón de franjas verticales. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BackgroundTypeDemo
    {
        public static void BackgroundTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo del libro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceda a una celda de la hoja de cálculo
            Cell cell = worksheet.Cells["A1"];
            
            // Establezca el valor de la celda
            cell.PutValue("Hello, Aspose!");

            // Cree un objeto de estilo
            Style style = cell.GetStyle();
            
            // Establezca el tipo de patrón de fondo
            style.Pattern = BackgroundType.DiagonalStripe;
            
            // Establezca el color de primer plano
            style.ForegroundColor = Color.Red;
            
            // Establezca el color de fondo
            style.BackgroundColor = Color.Green;
            
            // Aplique el estilo a la celda
            cell.SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("BackgroundTypeExample.xlsx");
            workbook.Save("BackgroundTypeExample.pdf");



        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


