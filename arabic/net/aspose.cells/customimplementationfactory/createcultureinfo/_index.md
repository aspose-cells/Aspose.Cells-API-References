---
title: "CustomImplementationFactory.CreateCultureInfo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CustomImplementationFactory. إنشاء CultureInfo واحد بالمعرف المعطى"
type: docs
url: /ar/net/aspose.cells/customimplementationfactory/createcultureinfo/
---
## CustomImplementationFactory.CreateCultureInfo method

إنشاء CultureInfo واحد باستخدام المعرف المعطى.

```csharp
public virtual CultureInfo CreateCultureInfo(int lcid)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| lcid | Int32 |  |

### قيمة الإرجاع

مثيل CultureInfo.

### ملاحظات

هذا التنفيذ مفيد في الحالات التالية: 1. قد لا تكون بعض الثقافات مدعومة في بيئة المستخدم وإنشاء CultureInfo المطلوب بالمعرف المعطى قد يسبب استثناء. لتجنب الاستثناء، يمكن للمستخدم تجاوز هذه الطريقة لتوفير مثيل CultureInfo صالح للثقافة غير المدعومة. 2. قد يرغب المستخدم في تحديد بعض الخصائص المخصصة لبعض الثقافات للحصول على النتيجة المتوقعة للتنسيق. لهذا الغرض يمكن للمستخدم تجاوز هذه الطريقة لتوفير مثيل CultureInfo مع الخصائص المحددة من قبل المستخدم. يرجى ملاحظة أن خاصية UseUserOverride في مثيل CultureInfo المعاد قد تؤثر على النتيجة المنسقة. إذا كانت false، قد يتم تجاوز بعض خصائص مثيل CultureInfo المعاد بواسطة محرك التنسيق المدمج لدينا وفقًا لمتطلبات التنسيق في السيناريوهات المختلفة. إذا كانت true، لن نقوم بتغيير أي من خصائصه وسنستخدمه لتنسيق القيم مباشرة. لذا، إذا كان المستخدم قد حدد خصائص مخصصة لمثيل CultureInfo المعاد، يرجى التأكد من أن UseUserOverride لها true.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class CustomImplementationFactoryMethodCreateCultureInfoWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // إنشاء مثيل من CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // استدعِ CreateCultureInfo بمعرف LCID صالح (1033 للإنجليزية - الولايات المتحدة)
                int lcid = 1033;
                CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);

                // عرض النتائج
                Console.WriteLine($"CultureInfo created successfully with LCID: {lcid}");
                Console.WriteLine($"Culture Name: {cultureInfo.Name}");
                Console.WriteLine($"Display Name: {cultureInfo.DisplayName}");
                Console.WriteLine($"English Name: {cultureInfo.EnglishName}");

                // عرض كيفية ضبط المصنع في CellsHelper
                CellsHelper.CustomImplementationFactory = factory;
                Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling CreateCultureInfo: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


