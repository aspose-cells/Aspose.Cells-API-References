---
title: "Clase ConditionalFormattingIcon"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ConditionalFormattingIcon. Representa el ícono personalizado de la regla de formato condicional"
type: docs
url: /es/net/aspose.cells/conditionalformattingicon/
---
## ConditionalFormattingIcon class

Representa el ícono personalizado de la regla de formato condicional.

```csharp
public class ConditionalFormattingIcon
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ImageData](../../aspose.cells/conditionalformattingicon/imagedata/) { get; } | Obtiene los datos del conjunto de íconos. |
| [Index](../../aspose.cells/conditionalformattingicon/index/) { get; set; } | Obtiene y establece el índice del ícono en el conjunto de íconos. |
| [Type](../../aspose.cells/conditionalformattingicon/type/) { get; set; } | Obtiene y establece el tipo de conjunto de íconos. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetImageData](../../aspose.cells/conditionalformattingicon/getimagedata/)(Cell) | Obtiene los datos de la imagen con la configuración de la celda. |
| static [GetIconImageData](../../aspose.cells/conditionalformattingicon/geticonimagedata/)(IconSetType, int) | Obtener los datos del conjunto de íconos |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconDemo
    {
        public static void ConditionalFormattingIconExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo del libro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener la colección de formatos condicionales
            ConditionalFormattingCollection cformattings = worksheet.ConditionalFormattings;
            
            // Agregar un nuevo formato condicional a la colección
            int index = cformattings.Add();
            
            // Acceder a la colección de condiciones de formato
            FormatConditionCollection fcs = cformattings[index];
            
            // Definir el área de celdas donde aplicar el formato condicional
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            
            // Agregar el área de celdas a la colección de condiciones de formato
            fcs.AddArea(ca);
            
            // Agregar una condición para usar conjuntos de íconos
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcs[conditionIndex];
            
            // Establecer el tipo de conjunto de íconos
            fc.IconSet.Type = IconSetType.Arrows3;

            // Personalizar los íconos individuales dentro del conjunto de íconos
            ConditionalFormattingIcon cfIcon0 = fc.IconSet.CfIcons[0];
            cfIcon0.Type = IconSetType.Arrows3;
            cfIcon0.Index = 0;

            ConditionalFormattingIcon cfIcon1 = fc.IconSet.CfIcons[1];
            cfIcon1.Type = IconSetType.ArrowsGray3;
            cfIcon1.Index = 1;

            ConditionalFormattingIcon cfIcon2 = fc.IconSet.CfIcons[2];
            cfIcon2.Type = IconSetType.Boxes5;
            cfIcon2.Index = 2;

            // Guarda el libro de trabajo
            workbook.Save("ConditionalFormattingIconExample.xlsx");
            workbook.Save("ConditionalFormattingIconExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


