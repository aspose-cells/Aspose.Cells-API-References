---
title: "PivotTable.RowRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Devuelve un objeto CellArea que representa el rango que contiene el área de fila en el informe de PivotTable. Solo lectura"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/rowrange/
---
## PivotTable.RowRange property

Devuelve un objeto CellArea que representa el rango que contiene el área de filas en el informe de la tabla dinámica. Solo lectura.

```csharp
public CellArea RowRange { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowRangeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo a partir del archivo Excel fuente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Actualizar todas las tablas dinámicas en el libro de trabajo
            workbook.Worksheets.RefreshAll();
            
            // Obtener la primera tabla dinámica de la primera hoja de cálculo
            PivotTable pivotTable = workbook.Worksheets[0].PivotTables[0];
            
            // Obtener el rango de fila de la tabla dinámica
            CellArea rowRange = pivotTable.RowRange;
            
            // Mostrar las coordenadas del rango de fila
            Console.WriteLine("PivotTable Row Range:");
            Console.WriteLine($"Start Row: {rowRange.StartRow}");
            Console.WriteLine($"End Row: {rowRange.EndRow}");
            Console.WriteLine($"Start Column: {rowRange.StartColumn}");
            Console.WriteLine($"End Column: {rowRange.EndColumn}");
            
            // Obtener el rango de columna de la tabla dinámica
            CellArea columnRange = pivotTable.ColumnRange;
            
            // Mostrar las coordenadas del rango de columna
            Console.WriteLine("\nPivotTable Column Range:");
            Console.WriteLine($"Start Row: {columnRange.StartRow}");
            Console.WriteLine($"End Row: {columnRange.EndRow}");
            Console.WriteLine($"Start Column: {columnRange.StartColumn}");
            Console.WriteLine($"End Column: {columnRange.EndColumn}");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


