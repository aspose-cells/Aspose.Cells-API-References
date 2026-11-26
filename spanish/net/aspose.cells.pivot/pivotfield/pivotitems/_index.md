---
title: "PivotField.PivotItems"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Obtiene los elementos pivot del campo PivotField."
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/pivotitems/
---
## PivotField.PivotItems property

Obtiene los elementos dinámicos del pivot field

```csharp
public PivotItemCollection PivotItems { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyPivotItemsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["A4"].Value = "A";
            worksheet.Cells["B4"].Value = 30;
            
            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Actualizar datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Obtenga el campo pivot y demuestre PivotItems
            PivotField field = pivotTable.RowFields[0];
            Console.WriteLine("Field Name: " + field.Name);
            Console.WriteLine("Total PivotItems: " + field.PivotItems.Count);
            
            // Mostrar todos los nombres de los elementos pivot
            foreach (PivotItem item in field.PivotItems)
            {
                Console.WriteLine("Item Name: " + item.Name);
            }
        }
    }
}
```

### Ver también

* class [PivotItemCollection](../../pivotitemcollection/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


