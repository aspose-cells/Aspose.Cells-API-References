---
title: "Cell.HtmlString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene y establece la cadena html que contiene datos y algunos formatos en esta celda"
type: docs
url: /es/net/aspose.cells/cell/htmlstring/
---
## Cell.HtmlString property

Obtiene y establece la cadena html que contiene datos y algunos formatos en esta celda.

```csharp
public string HtmlString { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHtmlStringDemo
    {
        public static void Run()
        {
            // Crear una instancia de libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la colección de celdas
            Cells cells = worksheet.Cells;
            
            // Establecer cadena HTML con formato en la celda A1
            cells["A1"].HtmlString = "This is <b>bold</b> and <i>italic</i> text<br>with a line break";
            
            // Guarda el libro de trabajo
            workbook.Save("HtmlStringDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


