---
title: "PivotField.RegionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Especifica la región de la tabla dinámica donde se muestra este campo"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/regiontype/
---
## PivotField.RegionType property

Especifica la región de la tabla dinámica donde se muestra este campo.

```csharp
public PivotFieldType RegionType { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyRegionTypeDemo
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
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Actualizar los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Obtener el primer campo pivote
            PivotField pivotField = pivotTable.RowFields[0];

            // Mostrar el valor actual de RegionType
            Console.WriteLine("Current RegionType value: " + pivotField.RegionType);

            // Demostrar cómo usar la propiedad RegionType
            if (pivotField.RegionType == PivotFieldType.Row)
            {
                Console.WriteLine("This pivot field is in the row area");
            }

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldRegionTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


