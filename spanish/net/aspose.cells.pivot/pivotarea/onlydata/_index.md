---
title: "PivotArea.OnlyData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotArea. Indica si solo se seleccionan los valores de datos en el área de datos de la vista para una selección de elemento y no se incluyen las etiquetas del elemento"
type: docs
url: /es/net/aspose.cells.pivot/pivotarea/onlydata/
---
## PivotArea.OnlyData property

Indica si solo se seleccionan los valores de datos (en el área de datos de la vista) para una selección de elemento y no se incluyen las etiquetas del elemento.

```csharp
public bool OnlyData { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyOnlyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["A3"].PutValue("Clothing");
            worksheet.Cells["A4"].PutValue("Food");
            
            worksheet.Cells["B1"].PutValue("Revenue");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(3000);
            worksheet.Cells["B4"].PutValue(2000);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Configurar el área de pivote
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true; // Key property demonstration
            pivotArea.IsRowGrandIncluded = false;

            // Configuración de salida
            Console.WriteLine("OnlyData property is set to: " + pivotArea.OnlyData);
            
            workbook.Save("PivotAreaOnlyDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


