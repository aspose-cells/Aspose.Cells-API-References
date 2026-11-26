---
title: "Worksheet.Index"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Obtiene el índice de la hoja en la colección de hojas de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/index/
---
## Worksheet.Index property

Obtiene el índice de la hoja en la colección de hojas de cálculo.

```csharp
public int Index { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIndexDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar tres hojas de cálculo
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Acceder a las hojas de cálculo por índice y demostrar la propiedad Index
            Console.WriteLine("Worksheet Index Demonstration:");
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                Console.WriteLine($"Worksheet Name: {sheet.Name}, Index: {sheet.Index}");
            }

            // Agregar algo de formato condicional para demostrar el uso del índice
            Worksheet firstSheet = workbook.Worksheets[0];
            int formatIndex = firstSheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = firstSheet.ConditionalFormattings[formatIndex];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Mostrar información del índice de formato condicional
            Console.WriteLine("\nConditional Formatting Indexes:");
            Console.WriteLine($"Worksheet Index: {firstSheet.Index}");
            Console.WriteLine($"Formatting Collection Index: {formatIndex}");
            Console.WriteLine($"First Condition Index: 0");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


