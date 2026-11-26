---
title: "Enumeración DataBarNegativeColorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.DataBarNegativeColorType enum. Especifica si se debe usar el mismo color de borde y relleno que las barras de datos positivas"
type: docs
url: /es/net/aspose.cells/databarnegativecolortype/
---
## DataBarNegativeColorType enumeration

Especifica si se debe usar el mismo color de borde y relleno que las barras de datos positivas.

```csharp
public enum DataBarNegativeColorType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Color | `0` | Utilizar el color especificado en el cuadro de diálogo Negative Value and Axis Setting o mediante el uso de las propiedades ColorType y BorderColorType del objeto NegativeBarFormat. |
| SameAsPositive | `1` | Utilizar el mismo color que las barras de datos positivas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarNegativeColorTypeDemo
    {
        public static void DataBarNegativeColorTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(-20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(-40);
            worksheet.Cells["A5"].PutValue(50);

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Establecer las propiedades de la barra de datos
            DataBar dataBar = fc.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Number;
            dataBar.MinCfvo.Value = -50;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Number;
            dataBar.MaxCfvo.Value = 50;
            dataBar.Color = System.Drawing.Color.Green;

            // Establecer las propiedades del formato de barra negativa
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = System.Drawing.Color.Red;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = System.Drawing.Color.Blue;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.SameAsPositive;

            // Guarda el libro de trabajo
            workbook.Save("DataBarNegativeColorTypeExample.xlsx");
            workbook.Save("DataBarNegativeColorTypeExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


