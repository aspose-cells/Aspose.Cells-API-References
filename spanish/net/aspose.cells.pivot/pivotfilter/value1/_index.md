---
title: "PivotFilter.Value1"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFilter. Obtiene el valor de cadena value1 del filtro pivote de etiqueta"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/value1/
---
## PivotFilter.Value1 property

Obtiene el valor de cadena 1 del filtro dinámico de etiqueta.

```csharp
public string Value1 { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyValue1Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Rellena la hoja de cálculo con datos de ejemplo
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Banana";
            cells["A4"].Value = "Orange";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;

            // Agregar una tabla dinámica
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B4", "D1", "SalesPivot");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Agregue un filtro pivote y establezca Value1
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.Value1 = "Apple"; // Filter for Apple products only

            // Actualizar y calcular datos
            pivot.RefreshData();
            pivot.CalculateData();

            // Guarda el libro de trabajo
            book.Save("PivotFilterValue1Demo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


