---
title: "Enumeración TextureType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.TextureType. Representa el tipo de textura predefinido."
type: docs
url: /es/net/aspose.cells.drawing/texturetype/
---
## TextureType enumeration

Representa el tipo de textura predefinida.

```csharp
public enum TextureType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| BlueTissuePaper | `0` | Representa el tipo de textura de papel tisú azul. |
| Bouquet | `1` | Representa el tipo de textura de ramo. |
| BrownMarble | `2` | Representa el tipo de textura de mármol marrón. |
| Canvas | `3` | Representa el tipo de textura de lienzo. |
| Cork | `4` | Representa el tipo de textura de corcho. |
| Denim | `5` | Representa el tipo de textura de denim. |
| FishFossil | `6` | Representa el tipo de textura de fósil de pez. |
| Granite | `7` | Representa el tipo de textura de granito. |
| GreenMarble | `8` | Representa el tipo de textura de mármol verde. |
| MediumWood | `9` | Representa el tipo de textura de madera media. |
| Newsprint | `10` | Representa el tipo de textura de papel periódico. |
| Oak | `11` | Representa el tipo de textura de roble. |
| PaperBag | `12` | Representa el tipo de textura de bolsa de papel. |
| Papyrus | `13` | Representa el tipo de textura de papiro. |
| Parchment | `14` | Representa el tipo de textura de pergamino. |
| PinkTissuePaper | `15` | Representa el tipo de textura de papel tisú rosa. |
| PurpleMesh | `16` | Representa el tipo de textura de malla púrpura. |
| RecycledPaper | `17` | Representa el tipo de textura de papel reciclado. |
| Sand | `18` | Representa el tipo de textura de arena. |
| Stationery | `19` | Representa el tipo de textura Stationery. |
| Walnut | `20` | Representa el tipo de textura Walnut Droplets. |
| WaterDroplets | `21` | Representa el tipo de textura Water Droplets. |
| WhiteMarble | `22` | Representa el tipo de textura White Marble. |
| WovenMat | `23` | Representa el tipo de textura Woven Mat. |
| Unknown | `24` | Representa el tipo de textura Unknown. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTextureTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Product A");
            sheet.Cells["A3"].PutValue("Product B");
            sheet.Cells["A4"].PutValue("Product C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accede a la primera serie y establece la textura para un punto
            ChartPoint point = chart.NSeries[0].Points[2];
            point.Area.FillFormat.Texture = TextureType.Stationery;

            // Guarda el libro de trabajo
            workbook.Save("TextureTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


