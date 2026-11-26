---
title: "PivotTable.ShowInCompactForm"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Organiza la vista de la tabla dinámica en forma compacta"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showincompactform/
---
## PivotTable.ShowInCompactForm method

Diseña la vista de la tabla dinámica en forma compacta.

```csharp
public void ShowInCompactForm()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowInCompactFormDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir de los datos de origen
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Product");
            sourceSheet.Cells["C1"].PutValue("Sales");
            
            sourceSheet.Cells["A2"].PutValue("Electronics");
            sourceSheet.Cells["B2"].PutValue("Laptop");
            sourceSheet.Cells["C2"].PutValue(1200);
            
            sourceSheet.Cells["A3"].PutValue("Electronics");
            sourceSheet.Cells["B3"].PutValue("Phone");
            sourceSheet.Cells["C3"].PutValue(800);
            
            sourceSheet.Cells["A4"].PutValue("Furniture");
            sourceSheet.Cells["B4"].PutValue("Chair");
            sourceSheet.Cells["C4"].PutValue(150);
            
            sourceSheet.Cells["A5"].PutValue("Furniture");
            sourceSheet.Cells["B5"].PutValue("Table");
            sourceSheet.Cells["C5"].PutValue(300);

            // Crear una hoja de cálculo de tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Agregar tabla dinámica
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("=Sheet1!A1:C5", "A3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Agregar campos a áreas
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Configurar la tabla dinámica para mostrarse en forma compacta
            pivotTable.ShowInCompactForm();
            
            // Calcular datos y actualizar
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableCompactFormDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


