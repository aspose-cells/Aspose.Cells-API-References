---
title: "Estructura CellArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.CellArea struct. Representa un área de celdas"
type: docs
url: /es/net/aspose.cells/cellarea/
---
## CellArea structure

Representa un área de celdas.

```csharp
public struct CellArea : IComparable
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea_1)(string, string) | Crea un área de celdas. |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea)(int, int, int, int) | Crea un área de celdas. |
| [CompareTo](../../aspose.cells/cellarea/compareto/)(object) | Compara dos objetos CellArea según su esquina superior izquierda. |
| override [ToString](../../aspose.cells/cellarea/tostring/)() | Devuelve una cadena que representa el objeto de área de celda actual. |

## Campos

| Nombre | Descripción |
| --- | --- |
| [EndColumn](../../aspose.cells/cellarea/endcolumn/) | Obtiene o establece la columna final de esta área. |
| [EndRow](../../aspose.cells/cellarea/endrow/) | Obtiene o establece la fila final de esta área. |
| [StartColumn](../../aspose.cells/cellarea/startcolumn/) | Obtiene o establece la columna inicial de esta área. |
| [StartRow](../../aspose.cells/cellarea/startrow/) | Obtiene o establece la fila inicial de esta área. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellAreaDemo
    {
        public static void CellAreaExample()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B5"].PutValue(20);
            worksheet.Cells["B8"].PutValue(50);
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C7"].PutValue(15);
            worksheet.Cells["C9"].PutValue(30);

            // Crear área de celda
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;

            // Agregar una regla de formato condicional a la hoja de cálculo
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "30");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Guarda el libro de trabajo
            workbook.Save("CellAreaExample.xlsx");
            workbook.Save("CellAreaExample.pdf");

            // Demostrar el método ToString
            Console.WriteLine(ca.ToString());

            // Demostrar el método CompareTo
            CellArea ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            int comparisonResult = ca.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


