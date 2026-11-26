---
title: "PivotField.ShowValuesSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Obtiene la configuración de visualización de valores cuando se utiliza el cálculo ShowDataAs"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/showvaluessetting/
---
## PivotField.ShowValuesSetting property

Obtiene la configuración de mostrar valores cuando se está utilizando el cálculo ShowDataAs.

```csharp
public PivotShowValuesSetting ShowValuesSetting { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowValuesSettingDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 3000;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 1500;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 2500;
            cells["A7"].Value = "Banana";
            cells["B7"].Value = 3500;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B7", "C10", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Agregar campos de fila y de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];
            
            // Configura ShowValuesSetting para mostrar como porcentaje del total
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            
            // Calcular y actualizar la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldShowValuesSettingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotShowValuesSetting](../../pivotshowvaluessetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


