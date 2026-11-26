---
title: "CustomImplementationFactory.CreateRandomInstance"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CustomImplementationFactory. Создаёт один экземпляр генератора случайных чисел"
type: docs
url: /ru/net/aspose.cells/customimplementationfactory/createrandominstance/
---
## CustomImplementationFactory.CreateRandomInstance method

Создайте один экземпляр генератора случайных чисел.

```csharp
public virtual Random CreateRandomInstance()
```

### Возвращаемое значение

экземпляр генератора случайных чисел

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomImplementationFactoryMethodCreateRandomInstanceDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Вызовите CreateRandomInstance, чтобы получить объект Random
                Random random = factory.CreateRandomInstance();

                // Продемонстрировать функциональность экземпляра Random
                Console.WriteLine("Random instance created successfully.");
                Console.WriteLine($"Sample random number: {random.Next(1, 100)}");
                Console.WriteLine($"Sample random double: {random.NextDouble():F4}");

                // Показать, что фабрика может использоваться с CellsHelper
                CellsHelper.CustomImplementationFactory = factory;
                Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling CreateRandomInstance: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


