---
title: "CustomImplementationFactory.CreateMemoryStream"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomImplementationFactory yöntemi. Bir MemoryStream örneği veya MemoryStream'in özel bir uygulamasını oluşturur"
type: docs
url: /tr/net/aspose.cells/customimplementationfactory/creatememorystream/
---
## CreateMemoryStream() {#creatememorystream}

MemoryStream'in bir örneğini veya MemoryStream'in özel bir uygulamasını oluşturun.

```csharp
public virtual MemoryStream CreateMemoryStream()
```

### Dönüş Değeri

MemoryStream örneği.

### Örnekler

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
                // CustomImplementationFactory bir örneği oluşturun
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Parametresiz CreateMemoryStream kullanımını gösterin
                MemoryStream stream1 = factory.CreateMemoryStream();
                Console.WriteLine($"MemoryStream created with default capacity. Length: {stream1.Length}");

                // Kapasite parametresiyle CreateMemoryStream kullanımını gösterin
                int capacity = 2048;
                MemoryStream stream2 = factory.CreateMemoryStream(capacity);
                Console.WriteLine($"MemoryStream created with capacity: {capacity}. Length: {stream2.Length}");

                // İşlevselliği göstermek için bazı veriler yazın
                byte[] data = System.Text.Encoding.UTF8.GetBytes("Sample data for MemoryStream");
                stream2.Write(data, 0, data.Length);
                Console.WriteLine($"Data written to MemoryStream. New length: {stream2.Length}");

                // Olası okuma için konumu sıfırlayın
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

### Ayrıca Bakınız

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateMemoryStream(int) {#creatememorystream_1}

MemoryStream'in bir örneğini veya MemoryStream'in özel bir uygulamasını oluşturun.

```csharp
public virtual MemoryStream CreateMemoryStream(int capacity)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kapasite | Int32 | MemoryStream için başlangıç kapasitesi |

### Dönüş Değeri

MemoryStream örneği.

### Örnekler

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
                // CustomImplementationFactory bir örneği oluşturun
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Kapasite parametresiyle CreateMemoryStream'ı çağırın
                int capacity = 4096;
                MemoryStream memoryStream = factory.CreateMemoryStream(capacity);

                // Oluşturulan MemoryStream hakkında bilgi gösterin
                Console.WriteLine($"MemoryStream created successfully with capacity: {capacity}");
                Console.WriteLine($"Initial length: {memoryStream.Length}");
                Console.WriteLine($"Initial capacity: {memoryStream.Capacity}");

                // İşlevselliği göstermek için bazı örnek veriler yazın
                byte[] sampleData = System.Text.Encoding.UTF8.GetBytes("Test data for MemoryStream");
                memoryStream.Write(sampleData, 0, sampleData.Length);
                Console.WriteLine($"Data written. New length: {memoryStream.Length}");

                // Olası okuma için konumu sıfırlayın
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

### Ayrıca Bakınız

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


