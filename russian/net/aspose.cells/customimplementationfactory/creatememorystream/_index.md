---
title: "CustomImplementationFactory.CreateMemoryStream"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CustomImplementationFactory. Создаёт один экземпляр MemoryStream или пользовательскую реализацию MemoryStream"
type: docs
url: /ru/net/aspose.cells/customimplementationfactory/creatememorystream/
---
## CreateMemoryStream() {#creatememorystream}

Создайте один экземпляр MemoryStream или пользовательскую реализацию MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream()
```

### Возвращаемое значение

Экземпляр MemoryStream.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CustomImplementationFactoryMethodCreateMemoryStreamDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Продемонстрировать CreateMemoryStream без параметров
                MemoryStream stream1 = factory.CreateMemoryStream();
                Console.WriteLine($"MemoryStream created with default capacity. Length: {stream1.Length}");

                // Продемонстрировать CreateMemoryStream с параметром capacity
                int capacity = 2048;
                MemoryStream stream2 = factory.CreateMemoryStream(capacity);
                Console.WriteLine($"MemoryStream created with capacity: {capacity}. Length: {stream2.Length}");

                // Записать некоторые данные для демонстрации функциональности
                byte[] data = System.Text.Encoding.UTF8.GetBytes("Sample data for MemoryStream");
                stream2.Write(data, 0, data.Length);
                Console.WriteLine($"Data written to MemoryStream. New length: {stream2.Length}");

                // Сбросить позицию для возможного чтения
                stream2.Position = 0;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CreateMemoryStream demonstration: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateMemoryStream(int) {#creatememorystream_1}

Создайте один экземпляр MemoryStream или пользовательскую реализацию MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream(int capacity)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| capacity | Int32 | Начальная ёмкость MemoryStream |

### Возвращаемое значение

Экземпляр MemoryStream.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CustomImplementationFactoryMethodCreateMemoryStreamWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Вызовите CreateMemoryStream с параметром capacity
                int capacity = 4096;
                MemoryStream memoryStream = factory.CreateMemoryStream(capacity);

                // Отобразить информацию о созданном MemoryStream
                Console.WriteLine($"MemoryStream created successfully with capacity: {capacity}");
                Console.WriteLine($"Initial length: {memoryStream.Length}");
                Console.WriteLine($"Initial capacity: {memoryStream.Capacity}");

                // Напишите некоторые примерные данные, чтобы продемонстрировать функциональность
                byte[] sampleData = System.Text.Encoding.UTF8.GetBytes("Test data for MemoryStream");
                memoryStream.Write(sampleData, 0, sampleData.Length);
                Console.WriteLine($"Data written. New length: {memoryStream.Length}");

                // Сбросить позицию для возможного чтения
                memoryStream.Position = 0;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling CreateMemoryStream: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


