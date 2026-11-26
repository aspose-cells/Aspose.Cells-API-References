---
title: "PivotTable.EnableDataValueEditing"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Especifica un valor booleano que indica si el usuario puede editar las celdas en el área de datos de la tabla dinámica. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/enabledatavalueediting/
---
## PivotTable.EnableDataValueEditing property

Especifica un valor booleano que indica si se permite al usuario editar las celdas en el área de datos de la pivottable. El valor predeterminado es falso.

```csharp
public bool EnableDataValueEditing { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyEnableDataValueEditingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B5"].PutValue(3000);

            // Agregar una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Mostrar el valor actual de EnableDataValueEditing
            Console.WriteLine("Current EnableDataValueEditing value: " + pivotTable.EnableDataValueEditing);

            // Habilitar la edición de valores de datos
            pivotTable.EnableDataValueEditing = true;

            // Calcular datos para rellenar la tabla dinámica
            pivotTable.CalculateData();

            // Guardar el libro de trabajo antes de editar
            workbook.Save("PivotTableBeforeEdit.xlsx");

            // Ahora podemos editar los valores de datos directamente en la tabla dinámica
            // Para demostración, modificaremos una celda en el área de datos
            Cell dataCell = worksheet.Cells["F5"]; // Assuming this is a data cell
            if (dataCell != null)
            {
                dataCell.PutValue(2500); // Modify the value
            }

            // Guardar el libro de trabajo después de editar
            workbook.Save("PivotTableAfterEdit.xlsx");

            // Desactivar la edición de valores de datos
            pivotTable.EnableDataValueEditing = false;
            Console.WriteLine("EnableDataValueEditing set to: " + pivotTable.EnableDataValueEditing);
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


