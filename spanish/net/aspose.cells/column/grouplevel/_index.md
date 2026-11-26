---
title: "Column.GroupLevel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Column. Obtiene el nivel de agrupación de la columna"
type: docs
url: /es/net/aspose.cells/column/grouplevel/
---
## Column.GroupLevel property

Obtiene el nivel de grupo de la columna.

```csharp
public byte GroupLevel { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agrupar columnas (parámetro isHidden establecido en false)
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // Obtener el nivel de agrupación de la primera columna
            int groupLevel = worksheet.Cells.Columns[0].GroupLevel;
            
            // Mostrar el nivel de agrupación
            Console.WriteLine("Group level of first column: " + groupLevel);
            
            // Guarda el libro de trabajo
            workbook.Save("GroupLevelDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


