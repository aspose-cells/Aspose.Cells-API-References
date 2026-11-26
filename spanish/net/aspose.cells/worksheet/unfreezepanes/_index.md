---
title: "Worksheet.UnFreezePanes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Worksheet método. Descongela los paneles en la worksheet"
type: docs
url: /es/net/aspose.cells/worksheet/unfreezepanes/
---
## Worksheet.UnFreezePanes method

Descongela los paneles en la hoja de cálculo.

```csharp
public void UnFreezePanes()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnFreezePanesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Congelar paneles en la celda C3 (filas 2, columnas 2 congeladas)
            worksheet.FreezePanes("C3", 2, 2);

            // Verificar que los paneles están congelados
            int frozenRow, frozenColumn, frozenRows, frozenColumns;
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"Frozen panes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Descongelar los paneles
            worksheet.UnFreezePanes();

            // Verificar que los paneles están descongelados
            worksheet.GetFreezedPanes(out frozenRow, out frozenColumn, out frozenRows, out frozenColumns);
            Console.WriteLine($"After UnFreezePanes - Row: {frozenRow}, Column: {frozenColumn}, Rows: {frozenRows}, Columns: {frozenColumns}");

            // Guarda el libro de trabajo
            workbook.Save("UnFreezePanesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


