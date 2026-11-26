---
title: "ConditionalFormattingValue.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConditionalFormattingValue. Obtenga o establezca el tipo de este objeto de valor de formato condicional. Establecer el tipo a FormatConditionValueType.Min o FormatConditionValueType.Max establecerá automáticamente Value a null"
type: docs
url: /es/net/aspose.cells/conditionalformattingvalue/type/
---
## ConditionalFormattingValue.Type property

Obtenga o establezca el tipo de este objeto de valor de formato condicional. Establecer el tipo a FormatConditionValueType.Min o FormatConditionValueType.Max establecerá automáticamente \"Value\" a null.

```csharp
public FormatConditionValueType Type { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValuePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet ws = workbook.Worksheets[0];

                // Agregue algunos datos de muestra (requeridos para que exista el formato condicional)
                ws.Cells["A1"].PutValue(10);
                ws.Cells["A2"].PutValue(20);
                ws.Cells["A3"].PutValue(30);

                // Cree una colección de formato condicional y añada una condición IconSet
                int cfIndex = ws.ConditionalFormattings.Add();
                FormatConditionCollection fcc = ws.ConditionalFormattings[cfIndex];

                int condIdx = fcc.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcc[condIdx];
                condition.IconSet.Type = IconSetType.Arrows3; // any valid icon set type

                // Obtenga una instancia de ConditionalFormattingValue de la colección IconSet
                ConditionalFormattingValue cfv = condition.IconSet.Cfvos[0];

                // Establezca el Type a Percent y asigne un valor correspondiente
                cfv.Type = FormatConditionValueType.Percent;
                cfv.Value = 25; // 25%

                // Lea y muestre el Type y Value
                Console.WriteLine("After setting Type to Percent:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + cfv.Value);

                // Cambie el Type a Min – según la documentación, esto anulará Value
                cfv.Type = FormatConditionValueType.Min;

                // Lea y muestre nuevamente el Type y Value
                Console.WriteLine("\nAfter setting Type to Min:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + (cfv.Value == null ? "null" : cfv.Value.ToString()));

                // Guarde el libro de trabajo (el formato condicional es parte de la hoja)
                workbook.Save("ConditionalFormattingValueTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


