---
title: "PivotTable.AltTextDescription"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Obtiene la descripción del texto alternativo"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/alttextdescription/
---
## PivotTable.AltTextDescription property

Obtiene la descripción del texto alternativo.

```csharp
public string AltTextDescription { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyAltTextDescriptionDemo
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
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Crear una tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Mostrar la descripción actual del texto alternativo
            Console.WriteLine("Current AltTextDescription: " + pivotTable.AltTextDescription);

            // Establecer una nueva descripción del texto alternativo
            pivotTable.AltTextDescription = "Sales data by product category";

            // Guarda el libro de trabajo
            workbook.Save("PivotTableAltTextDescriptionDemo.xlsx");

            // Mostrar la nueva descripción del texto alternativo
            Console.WriteLine("New AltTextDescription: " + pivotTable.AltTextDescription);
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


