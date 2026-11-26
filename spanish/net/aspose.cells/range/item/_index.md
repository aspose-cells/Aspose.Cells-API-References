---
title: "Range.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene el objeto Cell en este rango"
type: docs
url: /es/net/aspose.cells/range/item/
---
## Range indexer

Obtiene el objeto [`Cell`](../../cell/) en este rango.

```csharp
public Cell this[int rowOffset, int columnOffset] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| rowOffset | Desplazamiento de fila en este rango, basado en cero. |
| columnOffset | Desplazamiento de columna en este rango, basado en cero. |

### Valor de retorno

[`Cell`](../../cell/) object.

### Ejemplos

```csharp
using System;
using System.Data;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RangePropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de ejemplo
            DataTable dt = new DataTable();
            dt.Columns.Add("Id", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Rows.Add(1001, "Item 1");
            dt.Rows.Add(1002, "Item 2");

            // Crea un rango y demuestra la propiedad Item
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B3");
            
            // Establece encabezados usando la propiedad Item
            range[0, 0].PutValue("Id");
            range[0, 1].PutValue("Name");

            // Llena datos usando la propiedad Item
            for (int i = 0; i < dt.Rows.Count; i++)
            {
                range[i + 1, 0].PutValue(dt.Rows[i]["Id"]);
                range[i + 1, 1].PutValue(dt.Rows[i]["Name"]);
            }

            // Formatea la fila de encabezado usando la propiedad Item
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.FromArgb(0, 176, 80);
            range[0, 0].SetStyle(style);
            range[0, 1].SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("RangePropertyItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


