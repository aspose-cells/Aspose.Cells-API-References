---
title: "Enumeración LookInType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.LookInType. Representa el tipo de búsqueda"
type: docs
url: /es/net/aspose.cells/lookintype/
---
## LookInType enumeration

Representa el tipo de inspección.

```csharp
public enum LookInType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Formulas | `0` | Busca el objeto buscado en la fórmula([`Formula`](../cell/formula/)) si la celda es una fórmula, de lo contrario lo busca en el valor original de la celda (igual que OriginalValues). |
| Values | `1` | Busca el objeto en el valor original de la celda([`Value`](../cell/value/)) y en el valor formateado([`StringValue`](../cell/stringvalue/)). |
| ValuesExcludeFormulaCell | `2` | Ignora las celdas que son fórmulas. Para aquellas celdas que no son fórmulas, es lo mismo que Values. |
| Comments | `3` | Busca el objeto solo en el comentario de la celda. Ignora aquellas celdas que no tienen comentario. |
| OnlyFormulas | `4` | Ignora las celdas que no son fórmulas. Para aquellas celdas que son fórmulas, busca el objeto buscado en la fórmula([`Formula`](../cell/formula/)). |
| OriginalValues | `5` | Busca el objeto solo en el valor original de la celda. |
| FormattedValues | `6` | Busca el objeto solo en el valor formateado de la celda([`StringValue`](../cell/stringvalue/)). |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassLookInTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos y fórmulas
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].Formula = "=A1";
            worksheet.Cells["C1"].PutValue("Contains B1");

            // Buscar celda que contiene la fórmula con "B1"
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            Cell foundCell = worksheet.Cells.Find("B1", null, options);

            // Mostrar el resultado
            if (foundCell != null)
            {
                Console.WriteLine($"Found cell at row: {foundCell.Row}, column: {foundCell.Column}");
                Console.WriteLine($"Cell value: {foundCell.StringValue}");
                Console.WriteLine($"Cell formula: {foundCell.Formula}");
            }
            else
            {
                Console.WriteLine("Cell not found");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


