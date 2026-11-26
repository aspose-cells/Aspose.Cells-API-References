---
title: "PivotItem.IsHidden"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotItem. Obtiene y establece si el elemento dinámico está oculto"
type: docs
url: /es/net/aspose.cells.pivot/pivotitem/ishidden/
---
## PivotItem.IsHidden property

Obtiene y establece si el elemento pivot está oculto.

```csharp
public bool IsHidden { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "债券借贷";
            worksheet.Cells["A3"].Value = "股票";
            worksheet.Cells["A4"].Value = "基金";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Acceder al campo dinámico y a los elementos
            PivotField field = pivotTable.RowFields[0];
            
            // Establecer la propiedad IsHidden para mostrar solo "债券借贷"
            foreach (PivotItem item in field.PivotItems)
            {
                item.IsHidden = (item.Name != "债券借贷");
            }

            // Actualizar tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotItemIsHiddenDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


