---
title: "FormatConditionCollection.GetCellArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FormatConditionCollection. Obtiene el rango de celdas con formato condicional por índice"
type: docs
url: /es/net/aspose.cells/formatconditioncollection/getcellarea/
---
## FormatConditionCollection.GetCellArea method

Obtiene el rango de celdas con formato condicional por índice.

```csharp
public CellArea GetCellArea(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | el índice del rango de celdas con formato condicional. |

### Valor de retorno

el rango de celdas con formato condicional

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodGetCellAreaWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = i + j;
                }
            }

            // Agregar formato condicional
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Establecer el rango del formato condicional
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 7;
            area.EndColumn = 3;
            fcc.AddArea(area);

            // Agregar condición y establecer estilo
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "10");
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            fcc[conditionIndex].Style = style;

            // Obtener y mostrar la información del área de la celda
            CellArea retrievedArea = fcc.GetCellArea(0);
            Console.WriteLine("Conditional Format Area:");
            Console.WriteLine($"StartRow: {retrievedArea.StartRow}");
            Console.WriteLine($"StartColumn: {retrievedArea.StartColumn}");
            Console.WriteLine($"EndRow: {retrievedArea.EndRow}");
            Console.WriteLine($"EndColumn: {retrievedArea.EndColumn}");

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


