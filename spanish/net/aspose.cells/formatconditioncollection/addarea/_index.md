---
title: "FormatConditionCollection.AddArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FormatConditionCollection. Agrega un rango de celdas con formato condicional"
type: docs
url: /es/net/aspose.cells/formatconditioncollection/addarea/
---
## FormatConditionCollection.AddArea method

Agrega un rango de celdas con formato condicional.

```csharp
public int AddArea(CellArea cellArea)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | CellArea | Rango de celdas con formato condicional. |

### Valor de retorno

Índice del rango de celdas con formato condicional.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue(row * col);
                }
            }

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection formatCollection = worksheet.ConditionalFormattings[index];
            
            // Crear condición de formato
            formatCollection.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Crear áreas de celdas y agregarlas a la colección de formatos
            CellArea area1 = CellArea.CreateCellArea(0, 0, 4, 4);
            CellArea area2 = CellArea.CreateCellArea(5, 5, 9, 9);
            
            formatCollection.AddArea(area1);
            formatCollection.AddArea(area2);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


