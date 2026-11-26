---
title: "PivotTable.MoveTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotTable. Mueve la PivotTable a una ubicación diferente en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/moveto/
---
## MoveTo(int, int) {#moveto}

Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo.

```csharp
public void MoveTo(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | índice de fila. |
| columna | Int32 | índice de columna. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["B3"].PutValue(2500);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");

            // Calcular datos para rellenar la tabla dinámica
            pivotTable.CalculateData();

            try
            {
                // Llamar al método MoveTo con parámetros (Int32, Int32) para mover la tabla dinámica
                pivotTable.MoveTo(5, 2); // Move to row 5, column 2
                
                Console.WriteLine("Pivot table moved successfully to new location (5,2)");
                
                // Calcular los datos nuevamente para actualizar la tabla dinámica movida
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing MoveTo method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("PivotTableMethodMoveToWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## MoveTo(int, int, int) {#moveto_1}

Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo.

```csharp
public void MoveTo(int sheetIndex, int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sheetIndex | Int32 | el índice de la hoja de cálculo de destino |
| fila | Int32 | índice de fila. |
| columna | Int32 | índice de columna. |

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## MoveTo(string) {#moveto_2}

Mueve la tabla dinámica a una ubicación diferente en la hoja de cálculo.

```csharp
public void MoveTo(string destCellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destCellName | String | el nombre de la celda de destino. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodMoveToWithStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Establecer datos de muestra
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";

            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;

            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;

            // Crear tabla dinámica
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            
            // Agregar campos a la tabla dinámica
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Establecer estilo y actualizar
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            sheet.RefreshPivotTables();

            // Mover la tabla dinámica a una nueva ubicación
            pivot.MoveTo("H16");
            sheet.RefreshPivotTables();

            // Guarda el libro de trabajo
            book.Save("PivotTableMoveToExample.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


