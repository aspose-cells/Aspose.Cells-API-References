---
title: "CellsHelper.CustomImplementationFactory"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsHelper. تحصل أو تعين المصنع لإنشاء مثيلات بتنفيذ خاص"
type: docs
url: /ar/net/aspose.cells/cellshelper/customimplementationfactory/
---
## CellsHelper.CustomImplementationFactory property

يحصل أو يعيّن المصنع لإنشاء مثيلات بتنفيذ خاص.

```csharp
public static CustomImplementationFactory CustomImplementationFactory { get; set; }
```

### أمثلة

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
            // إنشاء مثيل من CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // عرض طرق المصنع
            MemoryStream memoryStream = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            MemoryStream sizedStream = factory.CreateMemoryStream(1024);
            Console.WriteLine("MemoryStream created with capacity: 1024");

            CultureInfo culture = factory.CreateCultureInfo(1033);
            Console.WriteLine($"CultureInfo created: {culture.DisplayName}");

            Random random = factory.CreateRandomInstance();
            Console.WriteLine($"Random number generated: {random.Next()}");

            // تعيين المصنع في CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper");
        }
    }
}
```

### انظر أيضًا

* class [CustomImplementationFactory](../../customimplementationfactory/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


