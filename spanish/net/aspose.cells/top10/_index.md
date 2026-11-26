---
title: "Clase Top10"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Top10. Describe la regla de formato condicional Top10. Esta regla de formato condicional resalta las celdas cuyos valores se encuentran en el rango superior N o inferior N según lo especificado"
type: docs
url: /es/net/aspose.cells/top10/
---
## Top10 class

Describe la regla de formato condicional Top10. Esta regla de formato condicional resalta las celdas cuyos valores se encuentran en el rango superior N o inferior N, según se especifique.

```csharp
public class Top10
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Top10](top10/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IsBottom](../../aspose.cells/top10/isbottom/) { get; set; } | Obtener o establecer si una regla "top/bottom n" es una regla "bottom n". El valor predeterminado es false. |
| [IsPercent](../../aspose.cells/top10/ispercent/) { get; set; } | Obtener o establecer si una regla "top/bottom n" es una regla "top/bottom n percent". El valor predeterminado es false. |
| [Rank](../../aspose.cells/top10/rank/) { get; set; } | Obtener o establecer el valor de "n" en una regla de formato condicional "top/bottom n". Si IsPercent es true, el valor debe estar entre 0 y 100. De lo contrario debe estar entre 0 y 1000. El valor predeterminado es 10. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class Top10Demo
    {
        public static void Top10Example()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agrega un formato condicional vacío
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Establece el rango de formato condicional
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Agregar condición
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Estableciendo propiedades
            Top10 top10 = fc.Top10;
            top10.IsPercent = false;
            top10.IsBottom = false;
            top10.Rank = 5;

            // Guardando el archivo Excel
            workbook.Save("Top10Example.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


