---
title: "PivotTable.ShowInOutlineForm"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Dispone la PivotTable en forma de esquema"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showinoutlineform/
---
## PivotTable.ShowInOutlineForm method

Diseña la tabla dinámica en forma de esquema.

```csharp
public void ShowInOutlineForm()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInOutlineFormDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar hoja de cálculo con datos de muestra
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Agregar datos de ejemplo
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["B1"].PutValue("Product");
            dataSheet.Cells["C1"].PutValue("Sales");
            
            dataSheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            dataSheet.Cells["B2"].PutValue("Apple");
            dataSheet.Cells["C2"].PutValue(1000);
            
            dataSheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2));
            dataSheet.Cells["B3"].PutValue("Banana");
            dataSheet.Cells["C3"].PutValue(2000);
            
            dataSheet.Cells["A4"].PutValue(new DateTime(2023, 1, 3));
            dataSheet.Cells["B4"].PutValue("Apple");
            dataSheet.Cells["C4"].PutValue(1500);
            
            // Crear hoja de cálculo de tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Agregar tabla dinámica y obtener la referencia
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:C4", 
                "A3", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
                
            // Agregar campos a áreas
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Mostrar en forma de esquema
            pivotTable.ShowInOutlineForm();
            
            // Actualizar y calcular datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableOutlineFormDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


