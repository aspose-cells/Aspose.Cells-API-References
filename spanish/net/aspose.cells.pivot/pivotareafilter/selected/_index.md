---
title: "PivotAreaFilter.Selected"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotAreaFilter. Indica si este campo tiene selección. Solo funciona cuando la tabla dinámica está en vista de esquema"
type: docs
url: /es/net/aspose.cells.pivot/pivotareafilter/selected/
---
## PivotAreaFilter.Selected property

Indica si este campo tiene selección. Solo funciona cuando la PivotTable está en vista de esquema.

```csharp
public bool Selected { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterPropertySelectedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Crear una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Obtener filtro de área de tabla dinámica
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = pivotArea.Filters[0];

            // Mostrar el valor Selected actual
            Console.WriteLine("Current Selected value: " + filter.Selected);

            // Cambiar el valor Selected (solo afecta a la vista de esquema)
            filter.Selected = true;
            Console.WriteLine("New Selected value: " + filter.Selected);

            // Guarda el libro de trabajo
            workbook.Save("PivotAreaFilterSelectedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


