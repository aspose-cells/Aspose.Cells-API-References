---
title: "FormatCondition.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatCondition. Obtiene y establece si el tipo de formato condicional"
type: docs
url: /es/net/aspose.cells/formatcondition/type/
---
## FormatCondition.Type property

Obtiene y establece si el tipo de formato condicional.

```csharp
public FormatConditionType Type { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Crear formato condicional
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // Agregar condición de formato con tipo de expresión (parámetros corregidos)
            int conditionIndex = fcs.AddCondition(FormatConditionType.Expression, OperatorType.None, "=A1>5", null);
            FormatCondition fc = fcs[conditionIndex];
            
            // Establecer estilo para la condición
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            fc.Style = style;

            // Demostrar el uso de la propiedad Type
            Console.WriteLine("Format Condition Type: " + fc.Type);
            
            // Guarda el libro de trabajo
            workbook.Save("FormatConditionPropertyTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


