---
title: "Enum DataBarBorderType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.DataBarBorderType. Especifica el tipo de borde de una barra de datos."
type: docs
url: /es/net/aspose.cells/databarbordertype/
---
## DataBarBorderType enumeration

Especifica el tipo de borde de una barra de datos.

```csharp
public enum DataBarBorderType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | La barra de datos no tiene borde. |
| Solid | `1` | La barra de datos tiene un borde sólido. |

### Ejemplos

```csharp
using Aspose.Cells;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarBorderTypeDemo
    {
        public static void DataBarBorderTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Agregar formato condicional a la hoja de cálculo
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];

            // Definir un área de celdas para el formato condicional
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            // Agregar una regla de formato condicional de barra de datos
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];

            // Acceder al objeto DataBar
            DataBar dataBar = fc.DataBar;

            // Establecer el color de la barra de datos
            dataBar.Color = Color.Blue;

            // Establecer la longitud mínima y máxima de la barra de datos
            dataBar.MinLength = 10;
            dataBar.MaxLength = 90;

            // Establecer el tipo de borde de la barra de datos
            dataBar.BarBorder.Type = DataBarBorderType.Solid;

            // Establecer el color del borde de la barra de datos
            dataBar.BarBorder.Color = Color.Red;

            // Guarda el libro de trabajo
            workbook.Save("DataBarBorderTypeExample.xlsx");
            workbook.Save("DataBarBorderTypeExample.pdf");

            Console.WriteLine("DataBarBorderTypeExample executed successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


