---
title: "PivotTable.ShowDrill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Obtiene y establece si se muestran los botones de expandir/colapsar"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showdrill/
---
## PivotTable.ShowDrill property

Obtiene y establece si se muestran los botones de expandir/contraer.

```csharp
public bool ShowDrill { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowDrillDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y completarla con datos de ejemplo
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "Pivot";
            sheet.Cells["A1"].Value = "Category";
            sheet.Cells["B1"].Value = "Value";
            sheet.Cells["A2"].Value = "A";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["A3"].Value = "B";
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["A4"].Value = "A";
            sheet.Cells["B4"].Value = 150;

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Habilitar drilldown y mostrar indicadores de drill
            pivotTable.EnableDrilldown = true;
            pivotTable.ShowDrill = true;
            
            // Actualizar y calcular datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableShowDrillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


