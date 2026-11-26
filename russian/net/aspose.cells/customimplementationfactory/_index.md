---
title: "Класс CustomImplementationFactory"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CustomImplementationFactory. Фабрика для создания некоторых экземпляров, которые могут быть переопределены пользователем для особой цели"
type: docs
url: /ru/net/aspose.cells/customimplementationfactory/
---
## CustomImplementationFactory class

Фабрика для создания некоторых экземпляров, которые пользователь может переопределить для специальной цели.

```csharp
public class CustomImplementationFactory
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CustomImplementationFactory](customimplementationfactory/)() | Конструктор по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [CreateCultureInfo](../../aspose.cells/customimplementationfactory/createcultureinfo/)(int) | Создайте один CultureInfo по заданному идентификатору. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream)() | Создайте один экземпляр MemoryStream или пользовательскую реализацию MemoryStream. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream_1)(int) | Создайте один экземпляр MemoryStream или пользовательскую реализацию MemoryStream. |
| virtual [CreateRandomInstance](../../aspose.cells/customimplementationfactory/createrandominstance/)() | Создайте один экземпляр генератора случайных чисел. |

### Примеры

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
            // Создайте экземпляр CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Продемонстрируйте метод CreateMemoryStream без параметров
            MemoryStream memoryStream1 = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            // Продемонстрируйте метод CreateMemoryStream с параметром ёмкости
            int capacity = 1024;
            MemoryStream memoryStream2 = factory.CreateMemoryStream(capacity);
            Console.WriteLine($"MemoryStream created with capacity: {capacity}.");

            // Продемонстрируйте метод CreateCultureInfo
            int lcid = 1033; // LCID for English - United States
            CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);
            Console.WriteLine($"CultureInfo created with LCID: {lcid}.");

            // Продемонстрируйте метод CreateRandomInstance
            Random random = factory.CreateRandomInstance();
            Console.WriteLine("Random instance created.");

            // Пример использования фабрики с CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


