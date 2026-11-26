---
title: "WorkbookSettings.MaxColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene el índice máximo de columna basado en cero"
type: docs
url: /es/net/aspose.cells/workbooksettings/maxcolumn/
---
## WorkbookSettings.MaxColumn property

Obtiene el índice máximo de columna, basado en cero.

```csharp
public int MaxColumn { get; }
```

### Observaciones

Devuelve 255 si el formato de archivo es Excel97-2003;

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMaxColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Console.WriteLine("MaxColumn value: " + workbook.Settings.MaxColumn);
            
            // Demostrar el uso de MaxColumn intentando acceder a una columna más allá del límite
            try
            {
                Cells cells = workbook.Worksheets[0].Cells;
                Cell cell = cells[0, workbook.Settings.MaxColumn + 1];
                Console.WriteLine("This should not be reached");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error when accessing beyond MaxColumn: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


