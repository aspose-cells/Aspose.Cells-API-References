---
title: "DocumentProperty.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "DocumentProperty property. Obtiene o establece el valor de la propiedad"
type: docs
url: /es/net/aspose.cells.properties/documentproperty/value/
---
## DocumentProperty.Value property

Obtiene o establece el valor de la propiedad.

```csharp
public object Value { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a las propiedades de documento incorporadas
            var hyperlinkBase = workbook.Worksheets.BuiltInDocumentProperties["HyperlinkBase"];
            hyperlinkBase.Value = "http://www.example.com";

            var title = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            title.Value = "Sample Document Title";

            // Guarda el libro de trabajo
            workbook.Save("DocumentPropertiesDemo.xlsx");

            // Muestra los valores establecidos
            Console.WriteLine("HyperlinkBase: " + hyperlinkBase.Value);
            Console.WriteLine("Title: " + title.Value);
        }
    }
}
```

### Ver también

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


