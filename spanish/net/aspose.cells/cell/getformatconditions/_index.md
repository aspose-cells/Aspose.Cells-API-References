---
title: "Cell.GetFormatConditions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtiene las condiciones de formato que se aplican a esta celda"
type: docs
url: /es/net/aspose.cells/cell/getformatconditions/
---
## Cell.GetFormatConditions method

Obtiene las condiciones de formato que se aplican a esta celda.

```csharp
public FormatConditionCollection[] GetFormatConditions()
```

### Valor de retorno

Devuelve el objeto [`FormatConditionCollection`](../../formatconditioncollection/)

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetFormatConditionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener colección de celdas
            Cells cells = worksheet.Cells;
            
            // Agregar datos de ejemplo
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            
            // Agregar condición de formato a la celda A1
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
            
            // Obtener condiciones de formato para la celda A1
            FormatConditionCollection[] conditions = cells["A1"].GetFormatConditions();
            
            // Mostrar el número de condiciones de formato
            Console.WriteLine("Number of format conditions: " + conditions.Length);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


