---
title: "CellsHelper.CustomImplementationFactory"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellsHelper. Obtiene o establece la fábrica para crear instancias con implementación especial"
type: docs
url: /es/net/aspose.cells/cellshelper/customimplementationfactory/
---
## CellsHelper.CustomImplementationFactory property

Obtiene o establece la fábrica para crear instancias con implementación especial.

```csharp
public static CustomImplementationFactory CustomImplementationFactory { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyCustomImplementationFactoryDemo
    {
        public static void Run()
        {
            // Crea una instancia de CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Demostrar métodos de fábrica
            MemoryStream memoryStream = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            MemoryStream sizedStream = factory.CreateMemoryStream(1024);
            Console.WriteLine("MemoryStream created with capacity: 1024");

            CultureInfo culture = factory.CreateCultureInfo(1033);
            Console.WriteLine($"CultureInfo created: {culture.DisplayName}");

            Random random = factory.CreateRandomInstance();
            Console.WriteLine($"Random number generated: {random.Next()}");

            // Establecer la fábrica en CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper");
        }
    }
}
```

### Ver también

* class [CustomImplementationFactory](../../customimplementationfactory/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


