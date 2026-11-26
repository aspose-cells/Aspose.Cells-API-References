---
title: "FormatConditionCollection.RangeCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatConditionCollection. Obtiene el recuento de rangos con formato condicional"
type: docs
url: /es/net/aspose.cells/formatconditioncollection/rangecount/
---
## FormatConditionCollection.RangeCount property

Obtiene el recuento de rangos con formato condicional.

```csharp
public int RangeCount { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionPropertyRangeCountDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Agregar rangos usando el método AddArea en lugar de AddRange
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 3, EndColumn = 0 });
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "50");

            // Demostrar la propiedad RangeCount
            Console.WriteLine($"Number of ranges in FormatConditionCollection: {fcc.RangeCount}");
            
            // Validar RangeCount
            if (fcc.RangeCount < 1)
            {
                Console.WriteLine("Error: No ranges applied to conditional formatting");
            }
            else
            {
                Console.WriteLine("Conditional formatting ranges applied successfully");
            }
        }
    }
}
```

### Ver también

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


