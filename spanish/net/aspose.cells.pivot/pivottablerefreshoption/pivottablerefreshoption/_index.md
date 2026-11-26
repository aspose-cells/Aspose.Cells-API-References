---
title: "PivotTableRefreshOption.PivotTableRefreshOption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor PivotTableRefreshOption. Representa las opciones de actualización de la fuente de datos de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottablerefreshoption/pivottablerefreshoption/
---
## PivotTableRefreshOption constructor

Representa las opciones de actualización de la fuente de datos de la tabla dinámica.

```csharp
public PivotTableRefreshOption()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableRefreshOptionMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Apple";
            cells["B2"].Value = "North";            cells["C2"].Value = 1000;
            cells["A3"].Value = "Orange";            cells["B3"].Value = "South";            cells["C3"].Value = 2000;
            cells["A4"].Value = "Banana";            cells["B4"].Value = "East";            cells["C4"].Value = 3000;
            cells["A5"].Value = "Apple";            cells["B5"].Value = "South";            cells["C5"].Value = 4000;
            
            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Crear y configurar opciones de actualización usando el constructor
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption();
            refreshOption.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            
            // Actualizar la tabla dinámica con opciones
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableRefreshDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [PivotTableRefreshOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


