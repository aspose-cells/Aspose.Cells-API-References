---
title: "CustomImplementationFactory.CreateRandomInstance"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CustomImplementationFactory. إنشاء نسخة واحدة من مولد الأرقام العشوائية"
type: docs
url: /ar/net/aspose.cells/customimplementationfactory/createrandominstance/
---
## CustomImplementationFactory.CreateRandomInstance method

إنشاء مثيل واحد من مولد الأرقام العشوائية.

```csharp
public virtual Random CreateRandomInstance()
```

### قيمة الإرجاع

نسخة من مولد الأرقام العشوائية

### أمثلة

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
                // إنشاء مثيل من CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // استدعِ CreateRandomInstance للحصول على كائن Random
                Random random = factory.CreateRandomInstance();

                // أظهر وظيفة نسخة Random
                Console.WriteLine("Random instance created successfully.");
                Console.WriteLine($"Sample random number: {random.Next(1, 100)}");
                Console.WriteLine($"Sample random double: {random.NextDouble():F4}");

                // أظهر أن المصنع يمكن استخدامه مع CellsHelper
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

### انظر أيضًا

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


