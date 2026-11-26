---
title: "CellsHelper.CustomImplementationFactory"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsHelper. Получает или задает фабрику для создания экземпляров со специальной реализацией"
type: docs
url: /ru/net/aspose.cells/cellshelper/customimplementationfactory/
---
## CellsHelper.CustomImplementationFactory property

Получает или задает фабрику для создания экземпляров со специальной реализацией.

```csharp
public static CustomImplementationFactory CustomImplementationFactory { get; set; }
```

### Примеры

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
            // Создайте экземпляр CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Продемонстрировать методы фабрики
            MemoryStream memoryStream = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            MemoryStream sizedStream = factory.CreateMemoryStream(1024);
            Console.WriteLine("MemoryStream created with capacity: 1024");

            CultureInfo culture = factory.CreateCultureInfo(1033);
            Console.WriteLine($"CultureInfo created: {culture.DisplayName}");

            Random random = factory.CreateRandomInstance();
            Console.WriteLine($"Random number generated: {random.Next()}");

            // Установить фабрику в CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper");
        }
    }
}
```

### См. также

* class [CustomImplementationFactory](../../customimplementationfactory/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


