---
title: "PivotTable.TableRange2"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Devuelve un objeto CellArea que representa el rango que contiene todo el informe de la PivotTable, incluye campos de página. Solo lectura"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/tablerange2/
---
## PivotTable.TableRange2 property

Devuelve un objeto CellArea que representa el rango que contiene todo el informe de la tabla dinámica, incluye los campos de página. Solo lectura.

```csharp
public CellArea TableRange2 { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyTableRange2Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Agregar una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Calcular datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Obtener el TableRange2 que incluye toda la tabla dinámica
            CellArea tableRange2 = pivotTable.TableRange2;
            Console.WriteLine($"TableRange2: StartRow={tableRange2.StartRow}, StartColumn={tableRange2.StartColumn}, " +
                $"EndRow={tableRange2.EndRow}, EndColumn={tableRange2.EndColumn}");

            // Crear un rango basado en TableRange2
            Aspose.Cells.Range pivotRange = worksheet.Cells.CreateRange(
                tableRange2.StartRow, 
                tableRange2.StartColumn, 
                tableRange2.EndRow - tableRange2.StartRow + 1, 
                tableRange2.EndColumn - tableRange2.StartColumn + 1);

            // Mostrar la dirección del rango
            Console.WriteLine($"Pivot Table Range: {pivotRange.Address}");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


