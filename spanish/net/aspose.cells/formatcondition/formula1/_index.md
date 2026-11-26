---
title: "FormatCondition.Formula1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatCondition. Obtiene y establece el valor o expresión asociado al formato condicional"
type: docs
url: /es/net/aspose.cells/formatcondition/formula1/
---
## FormatCondition.Formula1 property

Obtiene y establece el valor o expresión asociado al formato condicional.

```csharp
public string Formula1 { get; set; }
```

### Observaciones

Por favor, agregue todas las áreas antes de establecer la fórmula. Para establecer la fórmula de esta condición, si el valor de entrada comienza con '=', se considerará una fórmula. De lo contrario se tomará como un valor simple (texto, número, booleano). Para valores de texto que comienzan con '=', el usuario puede ingresarlos como fórmula en el formato: "=\"=...\"".

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyFormula1Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["E1"].PutValue(50);
            
            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Establecer el rango y el tipo de condición
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.LessOrEqual, "=$E$1<=100", null);
            
            // Acceder y mostrar la propiedad Formula1
            FormatCondition fc = fcc[0];
            Console.WriteLine("Formula1: " + fc.Formula1);
        }
    }
}
```

### Ver también

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


