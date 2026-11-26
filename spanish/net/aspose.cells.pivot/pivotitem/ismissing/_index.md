---
title: "PivotItem.IsMissing"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotItem. Indica si el elemento fue eliminado de la fuente de datos"
type: docs
url: /es/net/aspose.cells.pivot/pivotitem/ismissing/
---
## PivotItem.IsMissing property

Indica si el elemento fue eliminado de la fuente de datos.

```csharp
public bool IsMissing { get; }
```

### Observaciones

True significa que este valor ha sido eliminado de la fuente de datos.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotItemPropertyIsMissingDemo
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

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Actualizar los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Obtenga el primer elemento pivot en el primer campo de fila
            PivotField rowField = pivotTable.RowFields[0];
            PivotItem pivotItem = rowField.PivotItems[0];

            // Muestre el valor de la propiedad IsMissing
            Console.WriteLine("IsMissing value for '{0}': {1}", pivotItem.Name, pivotItem.IsMissing);

            // Cree un escenario donde un elemento podría estar ausente
            worksheet.Cells["A5"].PutValue("Grape");
            worksheet.Cells["B5"].PutValue(4000);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Verifique si el elemento pivot original está ahora ausente
            Console.WriteLine("After data change - IsMissing value for '{0}': {1}", 
                pivotItem.Name, pivotItem.IsMissing);

            // Guarda el libro de trabajo
            workbook.Save("PivotItemIsMissingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


