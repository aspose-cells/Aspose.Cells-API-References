---
title: "PivotField.IsValueFields"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Indica si este campo representa campos de valores"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/isvaluefields/
---
## PivotField.IsValueFields property

Indica si este campo representa campos de valores.

```csharp
[Obsolete("Use PivotField.IsValuesField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsValueFields { get; }
```

### Observaciones

NOTA: Este método ahora está obsoleto. En su lugar, utilice la propiedad PivotField.IsValuesField. Este método será eliminado 12 meses después a partir de noviembre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyIsValueFieldsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Bike";
            worksheet.Cells["A4"].Value = "Car";
            worksheet.Cells["A5"].Value = "Car";
            worksheet.Cells["B2"].Value = "East";
            worksheet.Cells["B3"].Value = "West";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["B5"].Value = "West";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["C4"].Value = 3000;
            worksheet.Cells["C5"].Value = 4000;

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Agregar campo de columna
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");

            // Agregar campo de datos y obtenerlo de la colección DataFields
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];

            // Mostrar el valor de la propiedad IsValueFields
            Console.WriteLine("IsValueFields for data field: " + dataField.IsValueFields);

            // Intentar encontrar un campo que no sea de datos para mostrar que IsValueFields es falso
            foreach (PivotField field in pivotTable.RowFields)
            {
                Console.WriteLine("IsValueFields for row field '" + field.Name + "': " + field.IsValueFields);
            }

            // Guardar el resultado
            workbook.Save("PivotFieldPropertyIsValueFieldsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


