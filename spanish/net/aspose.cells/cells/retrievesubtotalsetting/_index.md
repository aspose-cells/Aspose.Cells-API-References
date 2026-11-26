---
title: "Cells.RetrieveSubtotalSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Recupera la configuración de subtotales del rango"
type: docs
url: /es/net/aspose.cells/cells/retrievesubtotalsetting/
---
## Cells.RetrieveSubtotalSetting method

Recupera la configuración de subtotales del rango.

```csharp
public SubtotalSetting RetrieveSubtotalSetting(CellArea ca)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | CellArea | El rango |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRetrieveSubtotalSettingWithCellAreaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para subtotales
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group1" : "Group2");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Crear subtotales
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // Recuperar la configuración de subtotales
            SubtotalSetting setting = worksheet.Cells.RetrieveSubtotalSetting(area);

            // Configuración de salida
            Console.WriteLine("GroupBy: " + setting.GroupBy);
            Console.WriteLine("Function: " + setting.SubtotalFunction);
            Console.WriteLine("SummaryBelowData: " + setting.SummaryBelowData);
            Console.WriteLine("TotalList: " + string.Join(",", setting.TotalList));
        }
    }
}
```

### Ver también

* class [SubtotalSetting](../../subtotalsetting/)
* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


