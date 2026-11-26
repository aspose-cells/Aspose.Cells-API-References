---
title: "WorkbookSettings.MaxRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene el índice máximo de fila con base cero"
type: docs
url: /es/net/aspose.cells/workbooksettings/maxrow/
---
## WorkbookSettings.MaxRow property

Obtiene el índice máximo de fila, basado en cero.

```csharp
public int MaxRow { get; }
```

### Observaciones

Devuelve 65535 si el formato de archivo es Excel97-2003;

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Demostrar la propiedad MaxRow
            Console.WriteLine("Maximum rows in worksheet: " + workbook.Settings.MaxRow);
            
            // Intentar acceder a una celda más allá de MaxRow (debe lanzar una excepción)
            try
            {
                Cell cell = worksheet.Cells[workbook.Settings.MaxRow + 1, 0];
                Console.WriteLine("This line shouldn't execute");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error when accessing beyond MaxRow: " + ex.Message);
            }
            
            // Crear un área de celdas usando MaxRow
            CellArea area = CellArea.CreateCellArea(0, 0, workbook.Settings.MaxRow, 0);
            Console.WriteLine("Created cell area from row 0 to MaxRow: " + area.EndRow);
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


