---
title: "PivotFilter.MemberPropertyFieldIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFilter. Obtiene el índice del campo de propiedad de miembro del filtro pivot"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/memberpropertyfieldindex/
---
## PivotFilter.MemberPropertyFieldIndex property

Obtiene el índice del campo de propiedad de miembro del filtro dinámico.

```csharp
public int MemberPropertyFieldIndex { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyMemberPropertyFieldIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Configurar datos de muestra
            sheet.Cells["A1"].Value = "Category";
            sheet.Cells["A2"].Value = "Fruit";
            sheet.Cells["A3"].Value = "Vegetable";
            sheet.Cells["A4"].Value = "Fruit";
            sheet.Cells["A5"].Value = "Vegetable";
            
            sheet.Cells["B1"].Value = "Product";
            sheet.Cells["B2"].Value = "Apple";
            sheet.Cells["B3"].Value = "Carrot";
            sheet.Cells["B4"].Value = "Banana";
            sheet.Cells["B5"].Value = "Potato";
            
            sheet.Cells["C1"].Value = "Price";
            sheet.Cells["C2"].Value = 10;
            sheet.Cells["C3"].Value = 5;
            sheet.Cells["C4"].Value = 8;
            sheet.Cells["C5"].Value = 3;

            // Crear tabla dinámica - corregido obteniendo la tabla dinámica de la colección
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            
            // Agregar filtro pivot y establecer MemberPropertyFieldIndex
            int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            filter.MemberPropertyFieldIndex = 1; // Using Product field as member property
            
            // Actualizar tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            workbook.Save("PivotFilterWithMemberPropertyFieldIndex.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


