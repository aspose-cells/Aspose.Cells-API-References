---
title: "Klasse CustomImplementationFactory"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CustomImplementationFactory Klasse. Fabrik zum Erstellen einiger Instanzen, die vom Benutzer für einen speziellen Zweck neu implementiert werden können"
type: docs
url: /de/net/aspose.cells/customimplementationfactory/
---
## CustomImplementationFactory class

Factory zum Erzeugen einiger Instanzen, die vom Benutzer für einen speziellen Zweck neu implementiert werden können.

```csharp
public class CustomImplementationFactory
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [CustomImplementationFactory](customimplementationfactory/)() | Der Standardkonstruktor. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [CreateCultureInfo](../../aspose.cells/customimplementationfactory/createcultureinfo/)(int) | Erstelle ein CultureInfo-Objekt anhand der angegebenen ID. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream)() | Erstellen Sie eine Instanz von MemoryStream oder einer benutzerdefinierten Implementierung von MemoryStream. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream_1)(int) | Erstellen Sie eine Instanz von MemoryStream oder einer benutzerdefinierten Implementierung von MemoryStream. |
| virtual [CreateRandomInstance](../../aspose.cells/customimplementationfactory/createrandominstance/)() | Erstellen Sie eine Instanz eines Zufallszahlengenerators. |

### Beispiele

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
            // Erstellen Sie eine Instanz von CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Demonstrieren Sie die Methode CreateMemoryStream ohne Parameter
            MemoryStream memoryStream1 = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            // Demonstrieren Sie die Methode CreateMemoryStream mit Kapazitätsparameter
            int capacity = 1024;
            MemoryStream memoryStream2 = factory.CreateMemoryStream(capacity);
            Console.WriteLine($"MemoryStream created with capacity: {capacity}.");

            // Demonstrieren Sie die Methode CreateCultureInfo
            int lcid = 1033; // LCID for English - United States
            CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);
            Console.WriteLine($"CultureInfo created with LCID: {lcid}.");

            // Demonstrieren Sie die Methode CreateRandomInstance
            Random random = factory.CreateRandomInstance();
            Console.WriteLine("Random instance created.");

            // Beispielhafte Verwendung der Fabrik mit CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


