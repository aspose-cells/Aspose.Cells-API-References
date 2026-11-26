---
title: "PivotFilterCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFilterCollection. Obtiene el objeto pivotfilter en el índice específico"
type: docs
url: /es/net/aspose.cells.pivot/pivotfiltercollection/item/
---
## PivotFilterCollection indexer

Obtiene el objeto pivotfilter en el índice específico.

```csharp
public PivotFilter this[int index] { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Agregar filtro de tabla dinámica usando el método PivotFilterCollection.Add
            pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[0]; // Using Item property via index
            filter.Name = "SampleFilter";
            filter.Value1 = "100";
            
            // Acceder al filtro usando la propiedad Item y mostrar información
            Console.WriteLine("Filter Name: " + pivotTable.PivotFilters[0].Name);
            Console.WriteLine("Filter Value1: " + pivotTable.PivotFilters[0].Value1);
            Console.WriteLine("Filter Type: " + pivotTable.PivotFilters[0].FilterType);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../../pivotfilter/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


