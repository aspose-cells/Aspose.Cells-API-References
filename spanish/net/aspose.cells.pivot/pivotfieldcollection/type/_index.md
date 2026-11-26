---
title: "PivotFieldCollection.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFieldCollection. Obtiene el tipo de los PivotFields"
type: docs
url: /es/net/aspose.cells.pivot/pivotfieldcollection/type/
---
## PivotFieldCollection.Type property

Obtiene el tipo de PivotFields.

```csharp
public PivotFieldType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldCollectionPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 7;

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotFieldCollection rowFields = pivotTable.RowFields;

            // Mostrar el tipo de la colección de campos pivot
            Console.WriteLine("PivotFieldCollection Type: " + rowFields.Type);

            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            PivotFieldCollection dataFields = pivotTable.DataFields;

            // Mostrar el tipo de la colección de campos de datos
            Console.WriteLine("DataFields Type: " + dataFields.Type);

            // Calcular datos y actualizar la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guardar el resultado
            workbook.Save("PivotFieldCollectionTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


