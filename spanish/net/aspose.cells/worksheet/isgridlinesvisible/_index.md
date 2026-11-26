---
title: "Worksheet.IsGridlinesVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene o establece un valor que indica si las líneas de cuadrícula son visibles. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/worksheet/isgridlinesvisible/
---
## Worksheet.IsGridlinesVisible property

Obtiene o establece un valor que indica si las líneas de cuadrícula son visibles. El valor predeterminado es true.

```csharp
public bool IsGridlinesVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsGridlinesVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer la visibilidad de las líneas de cuadrícula en true
            worksheet.IsGridlinesVisible = true;
            
            // Agregar algunos datos de ejemplo para ver las líneas de cuadrícula
            worksheet.Cells["A1"].PutValue("Gridlines Visible Example");
            worksheet.Cells["A2"].PutValue("This worksheet shows gridlines");
            
            // Ajustar automáticamente las columnas para una mejor visibilidad
            worksheet.AutoFitColumns();
            
            // Guarda el libro de trabajo
            workbook.Save("GridlinesVisibleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


