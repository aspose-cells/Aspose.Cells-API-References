---
title: "تعداد ReConnectionMethodType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.ExternalConnections.ReConnectionMethodType. يحدد ما يجب أن تفعله تطبيق الجداول الإلكترونية عندما يفشل الاتصال"
type: docs
url: /ar/net/aspose.cells.externalconnections/reconnectionmethodtype/
---
## ReConnectionMethodType enumeration

يحدد ما يجب أن يفعله تطبيق جدول البيانات عندما يفشل الاتصال.

```csharp
public enum ReConnectionMethodType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Required | `1` | عند التحديث، استخدم معلومات الاتصال الحالية وإذا تبين أنها غير صالحة فاحصل على معلومات اتصال محدثة، إذا كانت متوفرة من ملف الاتصال الخارجي. |
| Always | `2` | في كل تحديث احصل على معلومات اتصال محدثة من ملف الاتصال الخارجي، إذا كان متوفرًا، واستخدمها بدلاً من معلومات الاتصال الحالية. في هذه الحالة سيفشل تحديث البيانات إذا كان ملف الاتصال الخارجي غير متاح. |
| Never | `3` | لا تحصل أبدًا على معلومات اتصال محدثة من ملف الاتصال الخارجي حتى لو كان متوفرًا وحتى لو كانت معلومات الاتصال الحالية غير صالحة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassReConnectionMethodTypeDemo
    {
        public static void Run()
        {
            try
            {
                // عرض إنشاء واستخدام قيم تعداد ReConnectionMethodType
                ReConnectionMethodType method1 = ReConnectionMethodType.Required;
                ReConnectionMethodType method2 = ReConnectionMethodType.Always;
                ReConnectionMethodType method3 = ReConnectionMethodType.Never;

                Console.WriteLine("ReConnectionMethodType values:");
                Console.WriteLine($"Required: {(int)method1}");
                Console.WriteLine($"Always: {(int)method2}");
                Console.WriteLine($"Never: {(int)method3}");

                // إظهار الاستخدام في جملة switch
                Console.WriteLine("\nDemonstrating switch usage:");
                TestConnectionMethod(method1);
                TestConnectionMethod(method2);
                TestConnectionMethod(method3);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ReConnectionMethodType: {ex.Message}");
            }
        }

        private static void TestConnectionMethod(ReConnectionMethodType method)
        {
            switch (method)
            {
                case ReConnectionMethodType.Required:
                    Console.WriteLine("Using Required reconnection method");
                    break;
                case ReConnectionMethodType.Always:
                    Console.WriteLine("Using Always reconnection method");
                    break;
                case ReConnectionMethodType.Never:
                    Console.WriteLine("Using Never reconnection method");
                    break;
                default:
                    Console.WriteLine("Unknown reconnection method");
                    break;
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


