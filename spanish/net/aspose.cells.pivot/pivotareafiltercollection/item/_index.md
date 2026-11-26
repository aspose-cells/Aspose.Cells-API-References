---
title: "PivotAreaFilterCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotAreaFilterCollection. Obtiene el filtro de la lista por el índice"
type: docs
url: /es/net/aspose.cells.pivot/pivotareafiltercollection/item/
---
## PivotAreaFilterCollection indexer

Obtiene el filtro de la lista por el índice.

```csharp
public PivotAreaFilter this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El Índice |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            
            // Agregar tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregue campos a áreas pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Crear formato condicional
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;
            
            // Crear área de tabla dinámica y agregar filtros
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Value");
            pcf.PivotAreas.Add(pivotArea);
            
            // Demostrar el uso de la propiedad Item
            PivotAreaFilter filter = pivotArea.Filters[0];
            filter.IsSubtotalSet(PivotFieldSubtotalType.Automatic);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotAreaFilterCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotAreaFilter](../../pivotareafilter/)
* class [PivotAreaFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


