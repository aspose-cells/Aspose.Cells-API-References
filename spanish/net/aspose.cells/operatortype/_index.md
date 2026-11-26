---
title: "Enumeración OperatorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.OperatorType enum. Representa el tipo de operador del formato condicional y la validación de datos"
type: docs
url: /es/net/aspose.cells/operatortype/
---
## OperatorType enumeration

Representa el tipo de operador del formato condicional y la validación de datos.

```csharp
public enum OperatorType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Between | `0` | Representa el operador Between del formato condicional y la validación de datos. |
| Equal | `1` | Representa el operador Equal del formato condicional y la validación de datos. |
| GreaterThan | `2` | Representa el operador GreaterThan del formato condicional y la validación de datos. |
| GreaterOrEqual | `3` | Representa el operador GreaterOrEqual del formato condicional y la validación de datos. |
| LessThan | `4` | Representa el operador LessThan del formato condicional y la validación de datos. |
| LessOrEqual | `5` | Representa el operador LessOrEqual del formato condicional y la validación de datos. |
| None | `6` | Representa sin comparación. |
| NotBetween | `7` | Representa el operador NotBetween del formato condicional y la validación de datos. |
| NotEqual | `8` | Representa el operador NotEqual del formato condicional y la validación de datos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OperatorTypeDemo
    {
        public static void OperatorTypeExample()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un formato condicional vacío
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Establecer el rango del formato condicional
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Agregar una condición con OperatorType.Between
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "100");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Agregar otra condición con OperatorType.GreaterThan
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;

            // Guarda el libro de trabajo
            workbook.Save("OperatorTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


