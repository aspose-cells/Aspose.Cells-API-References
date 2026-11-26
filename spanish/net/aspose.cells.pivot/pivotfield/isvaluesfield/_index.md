---
title: "PivotField.IsValuesField"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si este campo representa el campo de valores"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/isvaluesfield/
---
## PivotField.IsValuesField property

Indica si este campo representa un campo de valores.

```csharp
public bool IsValuesField { get; }
```

### Observaciones

Solo funciona cuando hay dos o más campos de datos en la vista de tabla dinámica.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyIsValuesFieldDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["C1"].Value = "Sales";

            cells["A2"].Value = "Fruit";
            cells["B2"].Value = "Apple";
            cells["C2"].Value = 100;

            cells["A3"].Value = "Fruit";
            cells["B3"].Value = "Orange";
            cells["C3"].Value = 150;

            cells["A4"].Value = "Vegetable";
            cells["B4"].Value = "Carrot";
            cells["C4"].Value = 200;

            cells["A5"].Value = "Vegetable";
            cells["B5"].Value = "Potato";
            cells["C5"].Value = 250;

            // Agregar tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            try
            {
                // Obtener el campo de datos (Sales)
                PivotField dataField = pivotTable.DataFields[0];

                // Mostrar el valor de la propiedad IsValuesField
                Console.WriteLine("IsValuesField value: " + dataField.IsValuesField);

                // Obtener un campo de fila (Category) para comparación
                PivotField rowField = pivotTable.RowFields["Category"];
                Console.WriteLine("Row field IsValuesField value: " + rowField.IsValuesField);

                // Calcular datos y actualizar
                pivotTable.CalculateData();

                // Guarda el libro de trabajo
                workbook.Save("IsValuesFieldDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


