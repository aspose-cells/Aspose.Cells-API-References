---
title: "Worksheet.IsRowColumnHeadersVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Obtiene o establece un valor que indica si la hoja de cálculo mostrará los encabezados de filas y columnas. El valor predeterminado es verdadero"
type: docs
url: /es/net/aspose.cells/worksheet/isrowcolumnheadersvisible/
---
## Worksheet.IsRowColumnHeadersVisible property

Obtiene o establece un valor que indica si la hoja de cálculo mostrará los encabezados de filas y columnas. El valor predeterminado es true.

```csharp
public bool IsRowColumnHeadersVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRowColumnHeadersVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer la visibilidad de los encabezados de filas y columnas a falso
            worksheet.IsRowColumnHeadersVisible = false;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Cargar el libro de trabajo guardado para verificar la propiedad
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Mostrar el valor de la propiedad
            Console.WriteLine("Row and Column Headers Visible: " + loadedWorksheet.IsRowColumnHeadersVisible);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


