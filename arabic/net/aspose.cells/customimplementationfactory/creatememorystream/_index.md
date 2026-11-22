---
title: "CustomImplementationFactory.CreateMemoryStream"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CustomImplementationFactory. إنشاء نسخة واحدة من MemoryStream أو تنفيذ مخصص لـ MemoryStream"
type: docs
url: /ar/net/aspose.cells/customimplementationfactory/creatememorystream/
---
## CreateMemoryStream() {#creatememorystream}

إنشاء مثيل واحد من MemoryStream أو تنفيذ مخصص لـ MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream()
```

### قيمة الإرجاع

نسخة MemoryStream.

### أمثلة

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
                // إنشاء مثيل من CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // اعرض CreateMemoryStream بدون معلمات
                MemoryStream stream1 = factory.CreateMemoryStream();
                Console.WriteLine($"MemoryStream created with default capacity. Length: {stream1.Length}");

                // اعرض CreateMemoryStream مع معلمة السعة
                int capacity = 2048;
                MemoryStream stream2 = factory.CreateMemoryStream(capacity);
                Console.WriteLine($"MemoryStream created with capacity: {capacity}. Length: {stream2.Length}");

                // اكتب بعض البيانات لإظهار الوظيفة
                byte[] data = System.Text.Encoding.UTF8.GetBytes("Sample data for MemoryStream");
                stream2.Write(data, 0, data.Length);
                Console.WriteLine($"Data written to MemoryStream. New length: {stream2.Length}");

                // أعد تعيين الموضع للقراءة المحتملة
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

### انظر أيضًا

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateMemoryStream(int) {#creatememorystream_1}

إنشاء مثيل واحد من MemoryStream أو تنفيذ مخصص لـ MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream(int capacity)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| السعة | Int32 | السعة الأولية لـ MemoryStream |

### قيمة الإرجاع

نسخة MemoryStream.

### أمثلة

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
                // إنشاء مثيل من CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // استدعِ CreateMemoryStream مع معلمة السعة
                int capacity = 4096;
                MemoryStream memoryStream = factory.CreateMemoryStream(capacity);

                // اعرض معلومات حول MemoryStream المُنشأ
                Console.WriteLine($"MemoryStream created successfully with capacity: {capacity}");
                Console.WriteLine($"Initial length: {memoryStream.Length}");
                Console.WriteLine($"Initial capacity: {memoryStream.Capacity}");

                // اكتب بعض البيانات التجريبية لتوضيح الوظيفة
                byte[] sampleData = System.Text.Encoding.UTF8.GetBytes("Test data for MemoryStream");
                memoryStream.Write(sampleData, 0, sampleData.Length);
                Console.WriteLine($"Data written. New length: {memoryStream.Length}");

                // أعد تعيين الموضع للقراءة المحتملة
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

### انظر أيضًا

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


