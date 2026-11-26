---
title: "ConditionalFormattingValueCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ConditionalFormattingValueCollection. Obtén el elemento CFValueObject en el índice especificado"
type: docs
url: /es/net/aspose.cells/conditionalformattingvaluecollection/item/
---
## ConditionalFormattingValueCollection indexer

Obtén el elemento CFValueObject en el índice especificado.

```csharp
public ConditionalFormattingValue this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValueCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar datos de ejemplo
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(120);
                worksheet.Cells["A3"].PutValue(260);

                // Agregar formato condicional
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

                // Establecer el rango para el formato condicional
                CellArea ca = new CellArea
                {
                    StartRow = 0,
                    EndRow = 2,
                    StartColumn = 0,
                    EndColumn = 0
                };
                fcs.AddArea(ca);

                // Agregar una condición de conjunto de iconos
                int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcs[conditionIndex];
                IconSet iconSet = condition.IconSet;
                iconSet.Type = IconSetType.Arrows3;

                // Obtener la ConditionalFormattingValueCollection
                ConditionalFormattingValueCollection cfvos = iconSet.Cfvos;

                // Agregar un valor a la colección
                int valueIndex = cfvos.Add(FormatConditionValueType.Number, "50");

                // Demostrar el acceso a la propiedad Item (indexador)
                ConditionalFormattingValue cfv = cfvos[valueIndex];

                // Mostrar el valor de la propiedad Item
                Console.WriteLine($"Conditional Formatting Value at index {valueIndex}:");
                Console.WriteLine($"  Type: {cfv.Type}");
                Console.WriteLine($"  Value: {cfv.Value}");
                Console.WriteLine($"  IsGTE: {cfv.IsGTE}");

                // Guarda el libro de trabajo
                workbook.Save("ConditionalFormattingValueCollectionItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ConditionalFormattingValueCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


