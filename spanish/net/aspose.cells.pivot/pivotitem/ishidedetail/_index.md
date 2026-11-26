---
title: "PivotItem.IsHideDetail"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotItem. Obtiene y establece si el elemento de pivote oculta los detalles"
type: docs
url: /es/net/aspose.cells.pivot/pivotitem/ishidedetail/
---
## PivotItem.IsHideDetail property

Obtiene y establece si el elemento de pivote oculta los detalles.

```csharp
[Obsolete("Use PivotItem.IsDetailHidden property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHideDetail { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotItem.IsDetailHidden. Esta propiedad será eliminada 12 meses después, a partir de noviembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIsHideDetailDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            foreach (PivotItem pivotItem in pivotItems)
            {
                Console.WriteLine($"Original IsHideDetail: {pivotItem.IsHideDetail}");
                pivotItem.IsHideDetail = true;
                Console.WriteLine($"Modified IsHideDetail: {pivotItem.IsHideDetail}");
            }

            workbook.Save("PivotItemIsHideDetailDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


