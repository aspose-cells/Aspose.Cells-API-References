---
title: "PivotTable.RowHeaderCaption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Obtiene y establece el título personalizado del encabezado de fila en este PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/rowheadercaption/
---
## PivotTable.RowHeaderCaption property

Obtiene y establece el título personalizado del encabezado de fila en esta tabla dinámica.

```csharp
public string RowHeaderCaption { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowHeaderCaptionDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar hoja de datos
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Agregar datos de ejemplo
            var cells = dataSheet.Cells;
            cells["A1"].PutValue("State");
            cells["B1"].PutValue("City");
            cells["C1"].PutValue("Population");
            
            cells["A2"].PutValue("TN");
            cells["B2"].PutValue("Chennai");
            cells["C2"].PutValue("50");
            
            cells["A3"].PutValue("KL");
            cells["B3"].PutValue("Cochin");
            cells["C3"].PutValue("70");
            
            // Agregar hoja de tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Agregar tabla dinámica y obtener su índice
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:C3", 
                "A3", 
                "PivotTable");
            
            // Obtener la instancia de la tabla dinámica
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Configurar tabla dinámica
            pivotTable.RowHeaderCaption = "State"; // Demonstrating RowHeaderCaption property
            pivotTable.AddFieldToArea(PivotFieldType.Row, "State");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Population");
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableWithRowHeaderCaption.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


