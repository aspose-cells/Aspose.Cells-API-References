---
title: "SubtotalSetting.SummaryBelowData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SubtotalSetting. Indica si se agrega un resumen debajo de los datos"
type: docs
url: /es/net/aspose.cells/subtotalsetting/summarybelowdata/
---
## SubtotalSetting.SummaryBelowData property

Indica si se agrega un resumen debajo de los datos.

```csharp
public bool SummaryBelowData { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySummaryBelowDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Cree el área de celdas para subtotales
            CellArea area = CellArea.CreateCellArea("A1", "B5");

            // Aplique subtotales usando el método Cells.Subtotal con todos los parámetros requeridos
            worksheet.Cells.Subtotal(
                area, 
                0, 
                ConsolidationFunction.Sum, 
                new int[] { 1 }, 
                false, 
                false, 
                false);  // summaryBelowData parameter

            // Recupere la configuración para verificar SummaryBelowData
            SubtotalSetting retrievedSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // Muestre el valor de la propiedad SummaryBelowData
            Console.WriteLine("SummaryBelowData: " + retrievedSetting.SummaryBelowData);
        }
    }
}
```

### Ver también

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


