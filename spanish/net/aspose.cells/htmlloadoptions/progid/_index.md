---
title: "HtmlLoadOptions.ProgId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlLoadOptions. Obtiene el id del programa que crea el archivo. Solo para archivos MHT"
type: docs
url: /es/net/aspose.cells/htmlloadoptions/progid/
---
## HtmlLoadOptions.ProgId property

Obtiene el id del programa que crea el archivo. Solo para archivos MHT.

```csharp
public string ProgId { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyProgIdDemo
    {
        public static void Run()
        {
            // Crear opciones de carga HTML con formato MHTML
            HtmlLoadOptions options = new HtmlLoadOptions(LoadFormat.MHtml);
            
            // Obtener la propiedad ProgId
            Console.WriteLine("ProgId is: " + options.ProgId);

            // Crear otra instancia y obtener su ProgId
            HtmlLoadOptions wordOptions = new HtmlLoadOptions(LoadFormat.MHtml);
            Console.WriteLine("ProgId is: " + wordOptions.ProgId);
        }
    }
}
```

### Ver también

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


