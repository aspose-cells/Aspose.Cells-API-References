---
title: "PivotTable.NullString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Obtiene la cadena mostrada en celdas que contienen valores nulos cuando la propiedad DisplayNullString es verdadera. El valor predeterminado es una cadena vacía"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/nullstring/
---
## PivotTable.NullString property

Obtiene la cadena que se muestra en celdas que contienen valores nulos cuando la propiedad DisplayNullString es verdadera. El valor predeterminado es una cadena vacía.

```csharp
public string NullString { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyNullStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 3000;
            cells["A5"].Value = null; // Null value
            cells["B5"].Value = 4000;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Establecer la propiedad NullString y la configuración de visualización
            pivotTable.NullString = "(null)";
            pivotTable.DisplayNullString = true;

            // Actualizar los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTableNullStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


