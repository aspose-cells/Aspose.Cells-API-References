---
title: "Clase CustomImplementationFactory"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CustomImplementationFactory. Fábrica para crear algunas instancias que pueden ser reimplementadas por el usuario con un propósito especial"
type: docs
url: /es/net/aspose.cells/customimplementationfactory/
---
## CustomImplementationFactory class

Fábrica para crear algunas instancias que pueden ser reimplementadas por el usuario con un propósito especial.

```csharp
public class CustomImplementationFactory
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CustomImplementationFactory](customimplementationfactory/)() | El constructor predeterminado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [CreateCultureInfo](../../aspose.cells/customimplementationfactory/createcultureinfo/)(int) | Crea un CultureInfo a partir del id proporcionado. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream)() | Crea una instancia de MemoryStream o de una implementación personalizada de MemoryStream. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream_1)(int) | Crea una instancia de MemoryStream o de una implementación personalizada de MemoryStream. |
| virtual [CreateRandomInstance](../../aspose.cells/customimplementationfactory/createrandominstance/)() | Crea una instancia de generador de números aleatorios. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;
    using System.IO;

    public class CustomImplementationFactoryDemo
    {
        public static void CustomImplementationFactoryExample()
        {
            // Crea una instancia de CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Demuestra el método CreateMemoryStream sin parámetros
            MemoryStream memoryStream1 = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            // Demuestra el método CreateMemoryStream con el parámetro de capacidad
            int capacity = 1024;
            MemoryStream memoryStream2 = factory.CreateMemoryStream(capacity);
            Console.WriteLine($"MemoryStream created with capacity: {capacity}.");

            // Demuestra el método CreateCultureInfo
            int lcid = 1033; // LCID for English - United States
            CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);
            Console.WriteLine($"CultureInfo created with LCID: {lcid}.");

            // Demuestra el método CreateRandomInstance
            Random random = factory.CreateRandomInstance();
            Console.WriteLine("Random instance created.");

            // Ejemplo de uso de la fábrica con CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


