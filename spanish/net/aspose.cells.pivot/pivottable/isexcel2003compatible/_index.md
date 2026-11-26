---
title: "PivotTable.IsExcel2003Compatible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Especifica si la PivotTable es compatible con Excel2003 al actualizarla; si es true, una cadena debe tener como máximo 255 caracteres, por lo que si la cadena supera los 255 caracteres será truncada. Si es false, una cadena no tendrá la restricción mencionada. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/isexcel2003compatible/
---
## PivotTable.IsExcel2003Compatible property

Especifica si la PivotTable es compatible con Excel2003 al actualizar la PivotTable; si es verdadero, una cadena debe tener 255 caracteres o menos, por lo que si la cadena supera los 255 caracteres, se truncará. Si es falso, una cadena no tendrá la restricción mencionada. El valor predeterminado es verdadero.

```csharp
public bool IsExcel2003Compatible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsExcel2003CompatibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Agregar una hoja de cálculo y completarla con datos de ejemplo
            Worksheet dataSheet = wb.Worksheets[0];
            dataSheet.Name = "Data";
            dataSheet.Cells["A1"].Value = "Product";
            dataSheet.Cells["B1"].Value = "Description";
            dataSheet.Cells["C1"].Value = "Status";
            dataSheet.Cells["D1"].Value = "Date";
            
            // Agregar filas de datos de muestra
            dataSheet.Cells["A2"].Value = "Product1";
            dataSheet.Cells["B2"].Value = "Short description";
            dataSheet.Cells["C2"].Value = "Active";
            dataSheet.Cells["D2"].Value = DateTime.Now;
            
            dataSheet.Cells["A3"].Value = "Product2";
            dataSheet.Cells["B3"].Value = "Very long description that exceeds Excel 2003 limits when used in pivot tables";
            dataSheet.Cells["C3"].Value = "Inactive";
            dataSheet.Cells["D3"].Value = DateTime.Now.AddDays(-1);

            // Agregar una tabla dinámica
            Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:D3", "A4", false);
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Configurar campos de la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Description
            
            // Establecer modo de compatibilidad
            pivotTable.IsExcel2003Compatible = false; // Allow longer text in pivot tables
            
            // Actualizar y calcular datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            wb.Save("PivotTableExcel2003CompatibilityDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


