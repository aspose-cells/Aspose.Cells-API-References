---
title: "Metered.Metered"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor Metered. Inicializa una nueva instancia de esta clase"
type: docs
url: /es/net/aspose.cells/metered/metered/
---
## Metered constructor

Inicializa una nueva instancia de esta clase.

```csharp
public Metered()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodCtorDemo
    {
        public static void Run()
        {
            // Crea una instancia usando el constructor
            Metered metered = new Metered();

            // Establecer licencia metered
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // Crear un libro de trabajo simple para demostrar la funcionalidad
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Metered License Demo");
            
            // Guarda el libro de trabajo
            workbook.Save("MeteredDemoOutput.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### Ver también

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


