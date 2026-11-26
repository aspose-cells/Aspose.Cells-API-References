---
title: "PivotItem.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotItem. Obtiene el nombre del elemento pivot"
type: docs
url: /es/net/aspose.cells.pivot/pivotitem/name/
---
## PivotItem.Name property

Obtiene el nombre del elemento pivot.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            ws.Cells["A1"].Value = "Category";
            ws.Cells["B1"].Value = "Value";
            ws.Cells["A2"].Value = "债券借贷";
            ws.Cells["A3"].Value = "股票";
            ws.Cells["A4"].Value = "基金";
            ws.Cells["B2"].Value = 100;
            ws.Cells["B3"].Value = 200;
            ws.Cells["B4"].Value = 300;

            // Crear tabla dinámica
            int index = ws.PivotTables.Add("A1:B4", "D3", "PivotTable1");
            PivotTable pivotTable = ws.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Acceda a los elementos pivot y demuestre la propiedad Name
            PivotField field = pivotTable.RowFields[0];
            foreach (PivotItem item in field.PivotItems)
            {
                // Ocultar todos los elementos excepto "债券借贷"
                item.IsHidden = item.Name != "债券借贷";
                Console.WriteLine($"Pivot Item Name: {item.Name}, Hidden: {item.IsHidden}");
            }
            
            // Actualizar y guardar
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            wb.Save("PivotItemNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


