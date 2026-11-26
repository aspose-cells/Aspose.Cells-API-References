---
title: "BuiltInDocumentPropertyCollection.TotalEditingTime"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece el tiempo total de edición en minutos"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/totaleditingtime/
---
## BuiltInDocumentPropertyCollection.TotalEditingTime property

Obtiene o establece el tiempo total de edición en minutos.

```csharp
public double TotalEditingTime { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTotalEditingTimeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a las propiedades de documento integradas
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Establecer el tiempo total de edición en minutos
            builtInProperties.TotalEditingTime = 90.5;

            // Mostrar el tiempo de edición establecido
            Console.WriteLine("Total Editing Time: " + builtInProperties.TotalEditingTime + " minutes");

            // Guarda el libro de trabajo
            workbook.Save("TotalEditingTimeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


