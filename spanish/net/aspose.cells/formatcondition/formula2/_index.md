---
title: "FormatCondition.Formula2"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatCondition. Obtiene y establece el valor o expresión asociado al formato condicional"
type: docs
url: /es/net/aspose.cells/formatcondition/formula2/
---
## FormatCondition.Formula2 property

Obtiene y establece el valor o expresión asociado al formato condicional.

```csharp
public string Formula2 { get; set; }
```

### Observaciones

Por favor, agregue todas las áreas antes de establecer la fórmula. Para establecer la fórmula de esta condición, si el valor de entrada comienza con '=', se considerará una fórmula. De lo contrario se tomará como un valor simple (texto, número, booleano). Para valores de texto que comienzan con '=', el usuario puede ingresarlos como fórmula en el formato: "=\"=...\"".

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula2Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar formato condicional
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[index];
            
            // Definir el rango de celdas
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            
            // Agregar condición de formato con Formula2
            formatConditions.Add(area, 
                FormatConditionType.CellValue, 
                OperatorType.Between, 
                "=\"abc def\"", 
                "=\"a\"&\"b\"");

            // Obtener la condición de formato
            FormatCondition formatCondition = formatConditions[0];

            // Mostrar las fórmulas
            Console.WriteLine("Formula1: " + formatCondition.Formula1);
            Console.WriteLine("Formula2: " + formatCondition.Formula2);

            // Guarda el libro de trabajo
            workbook.Save("FormatConditionFormula2Demo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


