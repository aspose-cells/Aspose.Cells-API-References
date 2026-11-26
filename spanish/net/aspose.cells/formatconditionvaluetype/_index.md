---
title: "Enum FormatConditionValueType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.FormatConditionValueType enum. Tipo de valor de condición"
type: docs
url: /es/net/aspose.cells/formatconditionvaluetype/
---
## FormatConditionValueType enumeration

Tipo de valor de condición.

```csharp
public enum FormatConditionValueType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Formula | `0` | El valor mínimo/ intermedio / máximo para el degradado se determina mediante una fórmula. |
| Max | `1` | Indica que el valor máximo en el rango se usará como el valor máximo para el degradado. |
| Min | `2` | Indica que el valor mínimo en el rango se usará como el valor mínimo para el degradado. |
| Number | `3` | Indica que el valor mínimo / intermedio / máximo para el degradado se especifica mediante un valor numérico constante. |
| Percent | `4` | El valor indica que un porcentaje entre los valores mínimo y máximo en el rango se usará como el valor mínimo / intermedio / máximo para el degradado. |
| Percentile | `5` | El valor indica que una clasificación percentil en el rango se usará como el valor mínimo / intermedio / máximo para el degradado. |
| AutomaticMax | `6` | Indica que el valor máximo automático en el rango se usará como el valor máximo automático para el degradado. |
| AutomaticMin | `7` | Indica que el valor mínimo automático en el rango se usará como el valor mínimo automático para el degradado. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFormatConditionValueTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar condiciones de formato
            int formatConditionsIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatConditionsIndex];
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[conditionIndex];

            // Establecer propiedades del conjunto de iconos
            condition.IconSet.Type = IconSetType.Boxes5;
            condition.IconSet.ShowValue = false;
            condition.IconSet.Reverse = true;

            // Establecer valor de celda y aplicar formato
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Boxes5 Icon Set Example");

            // Acceder al tipo de valor de condición de formato
            FormatConditionValueType valueType = condition.IconSet.Cfvos[0].Type;
            Console.WriteLine("First CFVO Type: " + valueType);

            // Mostrar valores de las condiciones del conjunto de iconos
            Console.WriteLine("\nIcon Set Threshold Values:");
            foreach (ConditionalFormattingValue cfvo in condition.IconSet.Cfvos)
            {
                Console.WriteLine($"Type: {cfvo.Type}, Value: {cfvo.Value}");
            }

            // Guarda el libro de trabajo
            workbook.Save("FormatConditionValueTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


