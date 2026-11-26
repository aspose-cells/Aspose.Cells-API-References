---
title: "SubtotalSetting.TotalList"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SubtotalSetting. Una matriz de desplazamientos de campo basados en cero que indican los campos a los que se añaden los subtotales"
type: docs
url: /es/net/aspose.cells/subtotalsetting/totallist/
---
## SubtotalSetting.TotalList property

Una matriz de desplazamientos de campo basados en cero, que indica los campos a los que se añaden los subtotales.

```csharp
public int[] TotalList { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertyTotalListDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Configuración de datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Cree y aplique el subtotal
            CellArea area = CellArea.CreateCellArea("A1", "B5");
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 }, true, true, true);

            // Recupere la configuración de subtotal para demostrar el uso de TotalList
            SubtotalSetting subtotal = worksheet.Cells.RetrieveSubtotalSetting(area);
            Console.WriteLine("TotalList contains column index: " + subtotal.TotalList[0]);
            
            // Guarda el libro de trabajo
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


