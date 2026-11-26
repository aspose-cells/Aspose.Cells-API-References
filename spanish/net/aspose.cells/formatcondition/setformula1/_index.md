---
title: "FormatCondition.SetFormula1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FormatCondition. Establece el valor o expresión asociado con esta condición de formato"
type: docs
url: /es/net/aspose.cells/formatcondition/setformula1/
---
## FormatCondition.SetFormula1 method

Establece el valor o expresión asociado a esta condición de formato.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
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

    public class FormatConditionMethodSetFormula1WithStringBooleanBooleanDemo
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

            // Agregar un rango de formato condicional
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Obtener la primera condición de formato
            FormatCondition fc = fcc[0];

            try
            {
                // Llamar a SetFormula1 con parámetros (String, Boolean, Boolean)
                fc.SetFormula1("SUM(A1:A4)", false, false);

                // Mostrar el resultado
                Console.WriteLine("SetFormula1 executed successfully with formula: " + fc.Formula1);
                Console.WriteLine("Conditional formatting applied to range A1:A4 with formula: " + fc.Formula1);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1 method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("FormatConditionSetFormula1Demo.xlsx");
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


