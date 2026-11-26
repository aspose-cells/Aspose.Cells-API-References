---
title: "PivotTable.AltTextTitle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Obtiene y establece el título del texto alternativo"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/alttexttitle/
---
## PivotTable.AltTextTitle property

Obtiene y establece el título del texto alternativo.

```csharp
public string AltTextTitle { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyAltTextTitleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);

            // Crear una tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "SalesPivotTable");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Mostrar el valor actual de AltTextTitle
            Console.WriteLine("Current AltTextTitle value: " + pivotTable.AltTextTitle);

            // Establecer un nuevo valor de AltTextTitle
            pivotTable.AltTextTitle = "Sales Data Pivot Table";

            // Calcular datos de tabla dinámica
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTableAltTextTitleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


