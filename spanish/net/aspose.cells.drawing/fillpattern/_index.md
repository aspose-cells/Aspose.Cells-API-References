---
title: "Enumeración FillPattern"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.FillPattern enum. Enumera los tipos de patrón de relleno de forma"
type: docs
url: /es/net/aspose.cells.drawing/fillpattern/
---
## FillPattern enumeration

Enumera los tipos de patrón de relleno de forma.

```csharp
public enum FillPattern
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Representa sin fondo. |
| Solid | `1` | Representa un patrón sólido. |
| Gray5 | `2` | Representa un patrón gris al 5%. |
| Gray10 | `3` | Representa un patrón gris al 10%. |
| Gray20 | `4` | Representa un patrón gris al 20%. |
| Gray30 | `5` | Representa un patrón gris al 30%. |
| Gray40 | `6` | Representa un patrón gris al 40%. |
| Gray50 | `7` | Representa un patrón gris del 50%. |
| Gray60 | `8` | Representa un patrón gris al 60%. |
| Gray70 | `9` | Representa un patrón gris al 70%. |
| Gray75 | `10` | Representa un patrón gris del 75%. |
| Gray80 | `11` | Representa el patrón gris al 80%. |
| Gray90 | `12` | Representa el patrón gris al 90%. |
| Gray25 | `13` | Representa un patrón gris del 25%. |
| LightDownwardDiagonal | `14` | Representa un patrón diagonal descendente claro. |
| LightUpwardDiagonal | `15` | Representa un patrón diagonal ascendente claro. |
| DarkDownwardDiagonal | `16` | Representa un patrón diagonal descendente oscuro. |
| DarkUpwardDiagonal | `17` | Representa un patrón diagonal ascendente oscuro. |
| WideDownwardDiagonal | `18` | Representa un patrón diagonal descendente ancho. |
| WideUpwardDiagonal | `19` | Representa un patrón diagonal ascendente ancho. |
| LightVertical | `20` | Representa un patrón vertical claro. |
| LightHorizontal | `21` | Representa un patrón horizontal claro. |
| NarrowVertical | `22` | Representa un patrón vertical estrecho. |
| NarrowHorizontal | `23` | Representa un patrón horizontal estrecho. |
| DarkVertical | `24` | Representa un patrón vertical oscuro. |
| DarkHorizontal | `25` | Representa un patrón horizontal oscuro. |
| DashedDownwardDiagonal | `26` | Representa un patrón diagonal descendente punteado. |
| DashedUpwardDiagonal | `27` | Representa un patrón diagonal ascendente punteado. |
| DashedVertical | `28` | Representa un patrón vertical punteado. |
| DashedHorizontal | `29` | Representa un patrón horizontal punteado. |
| SmallConfetti | `30` | Representa un patrón de confeti pequeño. |
| LargeConfetti | `31` | Representa un patrón de confeti grande. |
| ZigZag | `32` | Representa un patrón de zigzag. |
| Wave | `33` | Representa un patrón de onda. |
| DiagonalBrick | `34` | Representa un patrón de ladrillos diagonal. |
| HorizontalBrick | `35` | Representa un patrón de ladrillos horizontal. |
| Weave | `36` | Representa un patrón de tejido. |
| Plaid | `37` | Representa el patrón a cuadros. |
| Divot | `38` | Representa el patrón de hendidura. |
| DottedGrid | `39` | Representa el patrón de cuadrícula punteada. |
| DottedDiamond | `40` | Representa el patrón de diamante punteado. |
| Shingle | `41` | Representa el patrón de tejas. |
| Trellis | `42` | Representa el patrón de enrejado. |
| Sphere | `43` | Representa el patrón de esfera. |
| SmallGrid | `44` | Representa el patrón de cuadrícula pequeña. |
| LargeGrid | `45` | Representa el patrón de cuadrícula grande. |
| SmallCheckerBoard | `46` | Representa el patrón de tablero de ajedrez pequeño. |
| LargeCheckerBoard | `47` | Representa el patrón de tablero de ajedrez grande. |
| OutlinedDiamond | `48` | Representa el patrón de diamante contorneado. |
| SolidDiamond | `49` | Representa el patrón de diamante sólido. |
| Unknown | `50` | Representa un patrón desconocido. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillPatternDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer el patrón de relleno para la primera serie
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Pattern = FillPattern.Plaid;

            // Guarda el libro de trabajo
            workbook.Save("FillPatternDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


