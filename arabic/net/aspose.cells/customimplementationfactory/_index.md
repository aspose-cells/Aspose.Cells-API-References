---
title: "الفئة CustomImplementationFactory"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.CustomImplementationFactory. مصنع لإنشاء بعض المثيلات التي قد يعيد المستخدم تنفيذها لغرض خاص"
type: docs
url: /ar/net/aspose.cells/customimplementationfactory/
---
## CustomImplementationFactory class

مصنع لإنشاء بعض المثيلات التي قد يعيد المستخدم تنفيذها لغرض خاص.

```csharp
public class CustomImplementationFactory
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CustomImplementationFactory](customimplementationfactory/)() | البناء الافتراضي. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [CreateCultureInfo](../../aspose.cells/customimplementationfactory/createcultureinfo/)(int) | إنشاء CultureInfo واحد باستخدام المعرف المعطى. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream)() | إنشاء مثيل واحد من MemoryStream أو تنفيذ مخصص لـ MemoryStream. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream_1)(int) | إنشاء مثيل واحد من MemoryStream أو تنفيذ مخصص لـ MemoryStream. |
| virtual [CreateRandomInstance](../../aspose.cells/customimplementationfactory/createrandominstance/)() | إنشاء مثيل واحد من مولد الأرقام العشوائية. |

### أمثلة

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
            // إنشاء مثيل من CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // عرض طريقة CreateMemoryStream بدون معلمات
            MemoryStream memoryStream1 = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            // عرض طريقة CreateMemoryStream مع معلمة السعة
            int capacity = 1024;
            MemoryStream memoryStream2 = factory.CreateMemoryStream(capacity);
            Console.WriteLine($"MemoryStream created with capacity: {capacity}.");

            // عرض طريقة CreateCultureInfo
            int lcid = 1033; // LCID for English - United States
            CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);
            Console.WriteLine($"CultureInfo created with LCID: {lcid}.");

            // عرض طريقة CreateRandomInstance
            Random random = factory.CreateRandomInstance();
            Console.WriteLine("Random instance created.");

            // مثال على استخدام المصنع مع CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


