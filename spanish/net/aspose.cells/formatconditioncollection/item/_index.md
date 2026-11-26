---
title: "FormatConditionCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FormatConditionCollection. Obtiene la condición de formato por índice"
type: docs
url: /es/net/aspose.cells/formatconditioncollection/item/
---
## FormatConditionCollection indexer

Obtiene la condición de formato por índice.

```csharp
public FormatCondition this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | el índice de la condición de formato a devolver. |

### Valor de retorno

la condición de formato

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar una colección de condiciones de formato
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            
            // Agregar una condición de formato
            fcc.Add(CellArea.CreateCellArea(0, 0, 0, 3),
                FormatConditionType.CellValue, OperatorType.Between, "=A1", "=B1");

            // Acceder a la primera condición de formato usando la propiedad Item
            FormatCondition condition = fcc[0];
            
            // Mostrar las fórmulas
            Console.WriteLine("Formula1: " + condition.Formula1);
            Console.WriteLine("Formula2: " + condition.Formula2);
            
            // Modificar las fórmulas usando la propiedad Item
            fcc[0].Formula1 = "=C1";
            fcc[0].Formula2 = "=D1";
            
            // Mostrar fórmulas modificadas
            Console.WriteLine("Modified Formula1: " + fcc[0].Formula1);
            Console.WriteLine("Modified Formula2: " + fcc[0].Formula2);
        }
    }
}
```

### Ver también

* class [FormatCondition](../../formatcondition/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


