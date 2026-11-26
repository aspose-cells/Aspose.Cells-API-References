---
title: "Clase DataBarBorder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.DataBarBorder. Representa el borde de las barras de datos especificadas por una regla de formato condicional"
type: docs
url: /es/net/aspose.cells/databarborder/
---
## DataBarBorder class

Representa el borde de las barras de datos especificado por una regla de formato condicional.

```csharp
public class DataBarBorder
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Color](../../aspose.cells/databarborder/color/) { get; set; } | Obtiene o establece el color del borde de las barras de datos especificadas por una regla de formato condicional. |
| [Type](../../aspose.cells/databarborder/type/) { get; set; } | Obtiene o establece el tipo de borde de las barras de datos especificadas por una regla de formato condicional. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarBorderDemo
    {
        public static void DataBarBorderExample()
        {
            // Creando un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Accediendo a la primera hoja de cálculo en el libro de trabajo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregando algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(80);
            worksheet.Cells["A4"].PutValue(60);
            worksheet.Cells["A5"].PutValue(30);

            // Agregando un formato condicional vacío
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Definiendo un área de celdas para formato condicional
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // Agregando una condición de tipo DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition formatCondition = fcs[conditionIndex];

            // Accediendo al DataBar
            DataBar dataBar = formatCondition.DataBar;

            // Estableciendo las propiedades del DataBar
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 0;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MaxCfvo.Value = 100;
            dataBar.ShowValue = true;

            // Accediendo y estableciendo las propiedades del DataBarBorder
            DataBarBorder dataBarBorder = dataBar.BarBorder;
            dataBarBorder.Type = DataBarBorderType.Solid;
            dataBarBorder.Color = Color.Black;

            // Guardando el archivo Excel
            workbook.Save("DataBarBorderExample.xlsx");
            workbook.Save("DataBarBorderExample.pdf");

            Console.WriteLine("DataBar border example created successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


