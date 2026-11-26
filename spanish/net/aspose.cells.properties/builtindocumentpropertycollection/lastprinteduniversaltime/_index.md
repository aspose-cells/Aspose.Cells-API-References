---
title: "BuiltInDocumentPropertyCollection.LastPrintedUniversalTime"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece la hora universal cuando el documento se imprimió por última vez"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/lastprinteduniversaltime/
---
## BuiltInDocumentPropertyCollection.LastPrintedUniversalTime property

Obtiene o establece la hora universal en que el documento se imprimió por última vez.

```csharp
public DateTime LastPrintedUniversalTime { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastPrintedUniversalTimeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a las propiedades de documento integradas
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Establecer la propiedad LastPrintedUniversalTime
            DateTime currentUtcTime = DateTime.UtcNow;
            builtInProperties.LastPrintedUniversalTime = currentUtcTime;

            // Mostrar el valor establecido
            Console.WriteLine("LastPrintedUniversalTime set to: " + builtInProperties.LastPrintedUniversalTime);

            // Guarda el libro de trabajo
            workbook.Save("LastPrintedUniversalTimeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


