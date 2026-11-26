---
title: "Font.IsNormalizeHeights"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Indica si la normalización de la altura que se aplicará al fragmento de texto"
type: docs
url: /es/net/aspose.cells/font/isnormalizeheights/
---
## Font.IsNormalizeHeights property

Indica si se debe aplicar la normalización de altura al tramo de texto.

```csharp
[Obsolete("Use TextOptions.IsNormalizeHeights property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsNormalizeHeights { get; set; }
```

### Observaciones

Solo para las fuentes de Shapes o Charts. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [`IsNormalizeHeights`](../../../aspose.cells.drawing.texts/textoptions/isnormalizeheights/) . Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsNormalizeHeightsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Style style = workbook.CreateStyle();
            Font font = style.Font;

            // Establecer la propiedad IsNormalizeHeights
            font.IsNormalizeHeights = true;
            Console.WriteLine("Font IsNormalizeHeights: " + font.IsNormalizeHeights);

            // Aplicar el estilo a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Test Text");

            // Verificar la propiedad
            Font cellFont = cell.GetStyle().Font;
            Console.WriteLine("Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);

            // Modificar la propiedad
            cellFont.IsNormalizeHeights = false;
            Console.WriteLine("Modified Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


