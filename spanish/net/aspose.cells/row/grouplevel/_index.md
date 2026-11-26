---
title: "Row.GroupLevel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Row. Obtiene el nivel de agrupación de la fila"
type: docs
url: /es/net/aspose.cells/row/grouplevel/
---
## Row.GroupLevel property

Obtiene el nivel de grupo de la fila.

```csharp
public byte GroupLevel { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrupar filas 4-6 (hidden = false)
            worksheet.Cells.GroupRows(3, 5, false);

            // Acceder al nivel de agrupación de la fila 4
            int groupLevel = worksheet.Cells.Rows[3].GroupLevel;
            Console.WriteLine("Group level of row 4: " + groupLevel);

            // Desagrupar las filas
            worksheet.Cells.UngroupRows(3, 5);
        }
    }
}
```

### Ver también

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


