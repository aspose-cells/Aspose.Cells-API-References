---
title: "FormatCondition.SetFormula2"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FormatCondition. Establece el valor o expresión asociado con esta condición de formato"
type: docs
url: /es/net/aspose.cells/formatcondition/setformula2/
---
## FormatCondition.SetFormula2 method

Establece el valor o expresión asociado a esta condición de formato.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fórmula | String | El valor o expresión asociado con esta condición de formato. Si el valor de entrada comienza con '=', se tomará como fórmula. De lo contrario se tomará como valor simple (texto, número, bool). Para valores de texto que comienzan con '=', el usuario puede ingresarlo como fórmula en el formato: "=\"=...\"". |
| isR1C1 | Booleano | Si la fórmula es una fórmula R1C1. |
| isLocal | Booleano | Si la fórmula está formateada según la configuración regional. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodSetFormula2WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Agregar una condición de formato
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Obtener la primera condición de formato
            FormatCondition fc = fcs[0];

            try
            {
                // Llamar a SetFormula2 con los parámetros (String, Boolean, Boolean)
                fc.SetFormula2("25", false, false);

                // Mostrar el resultado
                Console.WriteLine("SetFormula2 executed successfully. New Formula2: " + fc.Formula2);
                Console.WriteLine("Cells A1:A4 will be formatted if their values are between 10 and 25");

                // Aplicar algún estilo para que el efecto sea visible
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightGreen;
                fc.Style = style;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula2 method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("FormatConditionSetFormula2Demo.xlsx");
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


