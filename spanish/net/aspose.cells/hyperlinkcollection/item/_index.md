---
title: "HyperlinkCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HyperlinkCollection. Obtiene el elemento Hyperlink en el índice especificado"
type: docs
url: /es/net/aspose.cells/hyperlinkcollection/item/
---
## HyperlinkCollection indexer

Obtiene el elemento [`Hyperlink`](../../hyperlink/) en el índice especificado.

```csharp
public Hyperlink this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue un hipervínculo a la celda A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.example.com");
            
            // Accede al primer hipervínculo usando la propiedad Item y establece el texto de visualización
            worksheet.Hyperlinks[0].TextToDisplay = "Click Here";
            
            // Establece el estilo del hipervínculo (texto azul subrayado)
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.Underline = FontUnderlineType.Single;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### Ver también

* class [Hyperlink](../../hyperlink/)
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


