---
title: "SubtotalSetting.SubtotalFunction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SubtotalSetting. La función de subtotal"
type: docs
url: /es/net/aspose.cells/subtotalsetting/subtotalfunction/
---
## SubtotalSetting.SubtotalFunction property

La función de subtotal.

```csharp
public ConsolidationFunction SubtotalFunction { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySubtotalFunctionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group A" : "Group B");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Cree la configuración de subtotal recuperándola de datos existentes
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // Configure el subtotal - estas propiedades son de solo lectura en la API real
            // Así que usaremos el método Subtotal directamente con parámetros
            int groupBy = 0; // Group by first column
            ConsolidationFunction function = ConsolidationFunction.Sum;
            int[] subtotalColumns = new int[] {1}; // Subtotal on second column
            
            // Aplique subtotales
            worksheet.Cells.Subtotal(area, groupBy, function, subtotalColumns);

            // Verifique la propiedad SubtotalFunction de la configuración recuperada
            Console.WriteLine("Subtotal Function: " + subtotalSetting.SubtotalFunction);
            
            // Guarda el libro de trabajo
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


