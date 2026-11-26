---
title: "ConditionalFormattingValue.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConditionalFormattingValue. Obtenga o establezca el valor de este objeto de valor de formato condicional. Debe usarse junto con Type"
type: docs
url: /es/net/aspose.cells/conditionalformattingvalue/value/
---
## ConditionalFormattingValue.Value property

Obtenga o establezca el valor de este objeto de valor de formato condicional. Debe usarse junto con Type.

```csharp
public object Value { get; set; }
```

### Observaciones

Si el valor es una cadena y comienza con "=", se procesará como una fórmula; de lo contrario, lo procesaremos como un valor simple.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyValueDemo
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

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Crear formato condicional de conjunto de iconos
            int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcc[conditionIndex];
            condition.IconSet.Type = IconSetType.Arrows3;

            // Obtenga los objetos de valor de formato condicional
            ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

            // Establezca valores para los íconos
            cfvos[0].Type = FormatConditionValueType.Min;
            cfvos[0].Value = 0;
            
            cfvos[1].Type = FormatConditionValueType.Percent;
            cfvos[1].Value = 33;
            
            cfvos[2].Type = FormatConditionValueType.Percent;
            cfvos[2].Value = 67;

            // Demuestre el uso de la propiedad Value
            Console.WriteLine("First icon value: " + cfvos[0].Value);
            Console.WriteLine("Second icon value: " + cfvos[1].Value);
            Console.WriteLine("Third icon value: " + cfvos[2].Value);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


