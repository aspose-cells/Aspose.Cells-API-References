---
title: "Clase FormatCondition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.FormatCondition. Representa una condición de formato condicional"
type: docs
url: /es/net/aspose.cells/formatcondition/
---
## FormatCondition class

Representa la condición de formato condicional.

```csharp
public class FormatCondition
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage/) { get; } | Obtenga la instancia "AboveAverage" del formato condicional. La regla de la instancia predeterminada resalta celdas que están por encima del promedio para todos los valores en el rango. Válido solo para type = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale/) { get; } | Obtenga la instancia "ColorScale" del formato condicional. La instancia predeterminada es una "green-yellow-red" 3ColorScale. Válido solo para type = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar/) { get; } | Obtenga la instancia "DataBar" del formato condicional. El color de la instancia predeterminada es azul. Válido solo para type = DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1/) { get; set; } | Obtiene y establece el valor o expresión asociado al formato condicional. |
| [Formula2](../../aspose.cells/formatcondition/formula2/) { get; set; } | Obtiene y establece el valor o expresión asociado al formato condicional. |
| [IconSet](../../aspose.cells/formatcondition/iconset/) { get; } | Obtenga la instancia "IconSet" del formato condicional. El IconSetType de la instancia predeterminada es TrafficLights31. Válido solo para type = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator/) { get; set; } | Obtiene y establece el tipo de operador de formato condicional. |
| [Priority](../../aspose.cells/formatcondition/priority/) { get; set; } | La prioridad de esta regla de formato condicional. Este valor se utiliza para determinar qué formato debe evaluarse y renderizarse. Los valores numéricos más bajos tienen mayor prioridad que los valores numéricos más altos, donde '1' es la prioridad más alta. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue/) { get; set; } | True, ninguna regla con prioridad inferior puede aplicarse sobre esta regla, cuando esta regla se evalúa como verdadera. Solo se aplica a Excel 2007; |
| [Style](../../aspose.cells/formatcondition/style/) { get; set; } | Obtiene o establece el estilo de los rangos de celdas con formato condicional. |
| [Text](../../aspose.cells/formatcondition/text/) { get; set; } | El valor de texto en una regla de formato condicional "text contains". Válido solo para type = containsText, notContainsText, beginsWith y endsWith. El valor predeterminado es null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod/) { get; set; } | El período de tiempo aplicable en una regla de formato condicional "date occurrin". Válido solo para type = timePeriod. El valor predeterminado es TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10/) { get; } | Obtenga la instancia "Top10" del formato condicional. La regla de la instancia predeterminada resalta celdas cuyos valores están dentro del top 10. Válido solo para type = Top10. |
| [Type](../../aspose.cells/formatcondition/type/) { get; set; } | Obtiene y establece si el tipo de formato condicional. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1)(bool, bool) | Obtiene el valor o expresión asociado a esta condición de formato. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_2)(int, int) | Obtiene la fórmula del formato condicional de la celda. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1/#getformula1_1)(bool, bool, int, int) | Obtiene el valor o expresión del formato condicional de la celda. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2)(bool, bool) | Obtiene el valor o expresión asociado a esta condición de formato. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_2)(int, int) | Obtiene la fórmula del formato condicional de la celda. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2/#getformula2_1)(bool, bool, int, int) | Obtiene el valor o expresión del formato condicional de la celda. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1/)(string, bool, bool) | Establece el valor o expresión asociado a esta condición de formato. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2/)(string, bool, bool) | Establece el valor o expresión asociado a esta condición de formato. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas/)(string, string, bool, bool) | Establece el valor o expresión asociado a esta condición de formato. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionDemo
    {
        public static void FormatConditionExample()
        {
            // Crear un nuevo libro de trabajo.
            Workbook workbook = new Workbook();

            // Obtener la primera hoja de cálculo.
            Worksheet sheet = workbook.Worksheets[0];

            // Agrega un formato condicional vacío
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Establece el rango del formato condicional.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // Añade condición.
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            FormatCondition fc = fcs[conditionIndex];

            // Estableciendo propiedades
            fc.Formula1 = "=A2";
            fc.Formula2 = "100";
            fc.Operator = OperatorType.Between;
            fc.StopIfTrue = true;
            fc.Priority = 1;
            fc.Style.BackgroundColor = Color.Red;
            fc.Type = FormatConditionType.CellValue;

            // Demostrando otras propiedades
            fc.Text = "Sample Text";
            fc.TimePeriod = TimePeriodType.Today;

            // Guardando el archivo Excel
            workbook.Save("FormatConditionExample.xlsx");
            workbook.Save("FormatConditionExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


