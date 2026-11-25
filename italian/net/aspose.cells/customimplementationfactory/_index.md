---
title: "Classe CustomImplementationFactory"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.CustomImplementationFactory classe. Factory per creare alcune istanze che possono essere riimplementate dall'utente per uno scopo speciale"
type: docs
url: /it/net/aspose.cells/customimplementationfactory/
---
## CustomImplementationFactory class

Factory per creare alcune istanze che possono essere reimplementate dall'utente per uno scopo speciale.

```csharp
public class CustomImplementationFactory
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CustomImplementationFactory](customimplementationfactory/)() | Il costruttore predefinito. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [CreateCultureInfo](../../aspose.cells/customimplementationfactory/createcultureinfo/)(int) | Crea un oggetto CultureInfo con l'ID fornito. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream)() | Crea un'istanza di MemoryStream o di un'implementazione personalizzata di MemoryStream. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream_1)(int) | Crea un'istanza di MemoryStream o di un'implementazione personalizzata di MemoryStream. |
| virtual [CreateRandomInstance](../../aspose.cells/customimplementationfactory/createrandominstance/)() | Crea un'istanza di generatore di numeri casuali. |

### Esempi

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
            // Crea un'istanza di CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Dimostra il metodo CreateMemoryStream senza parametri
            MemoryStream memoryStream1 = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            // Dimostra il metodo CreateMemoryStream con parametro di capacità
            int capacity = 1024;
            MemoryStream memoryStream2 = factory.CreateMemoryStream(capacity);
            Console.WriteLine($"MemoryStream created with capacity: {capacity}.");

            // Dimostra il metodo CreateCultureInfo
            int lcid = 1033; // LCID for English - United States
            CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);
            Console.WriteLine($"CultureInfo created with LCID: {lcid}.");

            // Dimostra il metodo CreateRandomInstance
            Random random = factory.CreateRandomInstance();
            Console.WriteLine("Random instance created.");

            // Esempio di utilizzo della factory con CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


