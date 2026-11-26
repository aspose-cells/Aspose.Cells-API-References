---
title: "IconSet.Cfvos"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad IconSet. Obtener la instancia de CFValueObjects"
type: docs
url: /es/net/aspose.cells/iconset/cfvos/
---
## IconSet.Cfvos property

Obtener la instancia de CFValueObjects.

```csharp
public ConditionalFormattingValueCollection Cfvos { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetPropertyCfvosDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            try
            {
                // Agregar formato condicional
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

                // Establecer rango para formato condicional
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 9;
                area.EndColumn = 0;
                fcs.AddArea(area);

                // Agregar condición de conjunto de iconos
                int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcs[conditionIndex];

                // Establecer tipo de conjunto de iconos
                condition.IconSet.Type = IconSetType.TrafficLights31;

                // Acceder a la propiedad Cfvos (solo lectura)
                ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

                // Mostrar información sobre la colección Cfvos
                Console.WriteLine("Number of CFValueObjects in the collection: " + cfvos.Count);

                // Iterar a través de la colección y mostrar cada valor
                for (int i = 0; i < cfvos.Count; i++)
                {
                    ConditionalFormattingValue cfValue = cfvos[i];
                    Console.WriteLine($"CFValue {i + 1}: Type = {cfValue.Type}, Value = {cfValue.Value}");
                }

                // Guarda el libro de trabajo
                workbook.Save("IconSetCfvosDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon set conditional formatting.");
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

* class [ConditionalFormattingValueCollection](../../conditionalformattingvaluecollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


