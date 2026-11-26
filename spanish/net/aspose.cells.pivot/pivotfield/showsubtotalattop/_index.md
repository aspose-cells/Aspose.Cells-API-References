---
title: "PivotField.ShowSubtotalAtTop"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotField. Indica si se deben mostrar los subtotales en la parte superior o inferior de los elementos"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/showsubtotalattop/
---
## PivotField.ShowSubtotalAtTop property

Indica si se deben mostrar los subtotales en la parte superior o inferior de los elementos.

```csharp
public bool ShowSubtotalAtTop { get; set; }
```

### Observaciones

Solo funciona para los campos pivot en la región de filas cuando ShowInOutlineForm es verdadero.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowSubtotalAtTopDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Bikes";
            worksheet.Cells["B3"].Value = 1500;
            worksheet.Cells["A4"].Value = "Cars";
            worksheet.Cells["B4"].Value = 2000;
            worksheet.Cells["A5"].Value = "Cars";
            worksheet.Cells["B5"].Value = 2500;

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Agregar campo de fila y configurar la posición del subtotal
            PivotField rowField = pivotTable.RowFields[pivotTable.AddFieldToArea(PivotFieldType.Row, "Product")];
            rowField.ShowSubtotalAtTop = true; // Demonstrate the property
            rowField.IsAutoSubtotals = true;

            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldShowSubtotalAtTopDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


