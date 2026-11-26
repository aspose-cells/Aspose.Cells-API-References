---
title: "PivotTable.ShowInTabularForm"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotTable. Organiza la tabla dinámica en forma tabular"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showintabularform/
---
## PivotTable.ShowInTabularForm method

Diseña la tabla dinámica en forma tabular.

```csharp
public void ShowInTabularForm()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInTabularFormDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar hoja de datos
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Agregar datos de muestra para la tabla dinámica
            dataSheet.Cells["A1"].PutValue("Label");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);

            // Agregar hoja de tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Agregar tabla dinámica
            int pivotIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Agregar campos a la tabla dinámica
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Mostrar tabla dinámica en forma tabular
            pivotTable.ShowInTabularForm();
            
            // Actualizar y calcular los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableShowInTabularFormDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


