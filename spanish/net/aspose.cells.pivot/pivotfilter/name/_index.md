---
title: "PivotFilter.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFilter. Obtiene el nombre del filtro pivote"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/name/
---
## PivotFilter.Name property

Obtiene el nombre del filtro dinámico.

```csharp
public string Name { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyNameDemo
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
            cells["B2"].Value = 100;
            cells["B3"].Value = 200;
            cells["B4"].Value = 300;

            // Agregar una tabla dinámica
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B4", "D1", "SalesPivot");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Agregue y configure un filtro pivote
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.Name = "ProductFilter"; // Demonstrating Name property usage
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Actualice y calcule los datos pivote
            pivot.RefreshData();
            pivot.CalculateData();

            // Guarda el libro de trabajo
            book.Save("PivotFilterNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


