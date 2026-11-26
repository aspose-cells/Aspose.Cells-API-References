---
title: "PivotTable.IsMultipleFieldFilters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros establecidos en ellos"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/ismultiplefieldfilters/
---
## PivotTable.IsMultipleFieldFilters property

Especifica un valor booleano que indica si los campos de una PivotTable pueden tener varios filtros aplicados.

```csharp
[Obsolete("Use PivotTable.AllowMultipleFiltersPerField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsMultipleFieldFilters { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotTable.AllowMultipleFiltersPerField. Este método será eliminado 12 meses después desde diciembre de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyIsMultipleFieldFiltersDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["B2"].PutValue("Fruit");
            worksheet.Cells["B3"].PutValue("Fruit");
            worksheet.Cells["B4"].PutValue("Fruit");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["C4"].PutValue(3000);

            // Crear una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Mostrar el valor actual de IsMultipleFieldFilters
            Console.WriteLine("Current IsMultipleFieldFilters value: " + pivotTable.IsMultipleFieldFilters);

            // Establecer IsMultipleFieldFilters en true para permitir múltiples filtros por campo
            pivotTable.IsMultipleFieldFilters = true;
            Console.WriteLine("IsMultipleFieldFilters set to: " + pivotTable.IsMultipleFieldFilters);

            // Actualiza y calcula la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTablePropertyIsMultipleFieldFiltersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


