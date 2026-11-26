---
title: "PivotFilter.MeasureFldIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFilter. Obtiene el índice del campo de medida del filtro pivot"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/measurefldindex/
---
## PivotFilter.MeasureFldIndex property

Obtiene el índice del campo de medida del filtro pivote.

```csharp
[Obsolete("Use PivotFilter.ValueFieldIndex property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int MeasureFldIndex { get; set; }
```

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice la propiedad PivotFilter.ValueFieldIndex. Este método será eliminado 12 meses después, a partir de noviembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyMeasureFldIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Apple";
            worksheet.Cells["A5"].Value = "Orange";

            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;
            worksheet.Cells["B5"].Value = 400;

            // Obtenga la colección de tablas dinámicas y agregue una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Obtenga la colección de filtros y agregue un filtro
            int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            filter.MeasureFldIndex = 1;

            workbook.Save("PivotFilterMeasureFldIndexDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


