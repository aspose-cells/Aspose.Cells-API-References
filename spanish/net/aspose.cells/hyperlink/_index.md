---
title: "Clase Hyperlink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Hyperlink. Encapsula el objeto que representa un hipervínculo"
type: docs
url: /es/net/aspose.cells/hyperlink/
---
## Hyperlink class

Encapsula el objeto que representa un hipervínculo.

```csharp
public class Hyperlink
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Address](../../aspose.cells/hyperlink/address/) { get; set; } | Representa la dirección de un hipervínculo. |
| [Area](../../aspose.cells/hyperlink/area/) { get; } | Obtiene el rango del hipervínculo. |
| [LinkType](../../aspose.cells/hyperlink/linktype/) { get; } | Obtiene el tipo de enlace. |
| [ScreenTip](../../aspose.cells/hyperlink/screentip/) { get; set; } | Devuelve o establece el texto de ScreenTip para el hipervínculo especificado. |
| [TextToDisplay](../../aspose.cells/hyperlink/texttodisplay/) { get; set; } | Representa el texto que se mostrará para el hipervínculo especificado. El valor predeterminado es la dirección del hipervínculo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Delete](../../aspose.cells/hyperlink/delete/)() | Elimina este hipervínculo |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkDemo
    {
        public static void HyperlinkExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            
            // Añadiendo una nueva hoja de cálculo al objeto Workbook
            workbook.Worksheets.Add();
            
            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un hipervínculo a una URL en la celda "A1"
            int index = worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");
            
            // Obteniendo un hipervínculo por índice
            Hyperlink hyperlink = worksheet.Hyperlinks[index];
            
            // Estableciendo el texto de visualización de este hipervínculo
            hyperlink.TextToDisplay = "Aspose";
            
            // Estableciendo el texto de ScreenTip para el hipervínculo
            hyperlink.ScreenTip = "Visit Aspose Website";
            
            // Guardando el archivo Excel
            workbook.Save("HyperlinkExample.xlsx");
            workbook.Save("HyperlinkExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


