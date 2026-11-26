---
title: "PivotTable.Format"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotTable. Formatea el área seleccionada del PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/format/
---
## Format(PivotArea, Style) {#format_1}

Da formato al área seleccionada de la tabla dinámica.

```csharp
public void Format(PivotArea pivotArea, Style style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivotArea | PivotArea | El área de vista pivote seleccionada. |
| estilo | Estilo | La configuración formateada. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotTableMethodFormatWithPivotAreaStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["A4"].Value = "Truck";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 5000;
            worksheet.Cells["B3"].Value = 12000;
            worksheet.Cells["B4"].Value = 8000;

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calcular datos para rellenar la tabla dinámica
            pivotTable.CalculateData();

            // Crear un estilo para formatear
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Crear área pivote para formatear
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.AxisType = PivotFieldType.Data;

            try
            {
                // Aplicar formato al área pivote
                pivotTable.Format(pivotArea, style);
                
                Console.WriteLine("Format method executed successfully with parameters (PivotArea, Style)");
                
                // Guardar el libro de trabajo para mostrar el efecto
                workbook.Save("PivotTableFormatWithPivotAreaStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Format method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PivotArea](../../pivotarea/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Format(CellArea, Style) {#format}

Da formato al área seleccionada de la tabla dinámica.

```csharp
public void Format(CellArea ca, Style style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | CellArea | El rango de las celdas. |
| estilo | Estilo | El estilo |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotTableMethodFormatWithCellAreaStyleDemo
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
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campos de fila y de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calcular datos y rangos
            pivotTable.CalculateData();
            pivotTable.CalculateRange();

            // Crear un estilo para formatear
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Definir el área de celda a formatear (rango del cuerpo de datos)
            CellArea area = pivotTable.DataBodyRange;

            try
            {
                // Llamar al método Format con los parámetros CellArea y Style
                pivotTable.Format(area, style);
                
                Console.WriteLine("PivotTable formatted successfully with parameters (CellArea, Style)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error formatting PivotTable: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("PivotTableFormatWithCellAreaStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Format(int, int, Style) {#format_2}

Da formato a la celda en el área de la tabla dinámica

```csharp
public void Format(int row, int column, Style style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila de la celda |
| columna | Int32 | Índice de columna de la celda |
| estilo | Estilo | Estilo que se usará para formatear la celda |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatWithInt32Int32StyleDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);

            // Agregar tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campos al área de filas
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Calcular datos
            pivotTable.CalculateData();

            // Crear un estilo para formatear
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.LightBlue;
            style.Font.IsBold = true;

            // Formatear la celda de encabezado de la tabla dinámica (fila 2, columna 0 en coordenadas de tabla dinámica)
            pivotTable.Format(2, 0, style);

            // Guarda el libro de trabajo
            workbook.Save("PivotTableFormatDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


