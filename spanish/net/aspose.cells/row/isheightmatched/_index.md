---
title: "Row.IsHeightMatched"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Row. Indica si la altura de la fila coincide con la configuración de fuente predeterminada actual del libro de trabajo. Verdadero en esta propiedad también indica que la altura de la fila es automática sin un valor de altura personalizado establecido por el usuario"
type: docs
url: /es/net/aspose.cells/row/isheightmatched/
---
## Row.IsHeightMatched property

Indica si la altura de la fila coincide con la configuración de fuente predeterminada actual del libro. Verdadero en esta propiedad también indica que la altura de la fila es "automática" sin un valor de altura personalizado establecido por el usuario.

```csharp
public bool IsHeightMatched { get; set; }
```

### Observaciones

Cuando esta propiedad es verdadera, si el contenido de esta fila cambia, generalmente la altura de la fila necesita ser recalculada (por ejemplo mediante [`AutoFitRows`](../../worksheet/autofitrows/)) para obtener el mismo resultado que se muestra en MS Excel al abrir el libro de trabajo en él.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHeightMatchedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer datos de muestra y estilo para demostrar la coincidencia de la altura de la fila
            worksheet.Cells["A1"].PutValue("This is a test string to demonstrate row height matching");
            worksheet.Cells["B1"].PutValue("Another cell in the same row");
            
            // Aplicar ajuste de texto para forzar el ajuste de altura
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Ajustar automáticamente la fila para que coincida con la altura del contenido
            worksheet.AutoFitRow(0);
            
            // Comprobar si la altura de la fila coincide con su contenido
            Console.WriteLine("Is row height matched: " + worksheet.Cells.Rows[0].IsHeightMatched);
        }
    }
}
```

### Ver también

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


