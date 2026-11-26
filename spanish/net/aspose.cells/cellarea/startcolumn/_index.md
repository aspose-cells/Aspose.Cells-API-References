---
title: "CellArea.StartColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Campo CellArea. Obtiene o establece la columna inicial de esta área"
type: docs
url: /es/net/aspose.cells/cellarea/startcolumn/
---
## CellArea.StartColumn field

Obtiene o establece la columna inicial de esta área.

```csharp
public int StartColumn;
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaFieldStartColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establezca algunos datos iniciales
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);

            // Cree un CellArea y establezca su StartColumn
            CellArea area = new CellArea();
            area.StartRow = 1;
            area.EndRow = 3;
            area.StartColumn = 0; // Using StartColumn field
            area.EndColumn = 0;

            // Inserte una nueva columna desplazando las celdas existentes hacia abajo
            cells.InsertRange(area, ShiftType.Down);

            // Verificar el resultado
            Console.WriteLine("A1 value: " + cells["A1"].StringValue); // Should be empty
            Console.WriteLine("A2 value: " + cells["A2"].StringValue); // Should be "Header"
            Console.WriteLine("A3 value: " + cells["A3"].IntValue); // Should be 10
        }
    }
}
```

### Ver también

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


