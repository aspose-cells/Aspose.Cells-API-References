---
title: "ConnectionParameterCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConnectionParameterCollection. يسترجع عنصر ConnectionParameter في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.externalconnections/connectionparametercollection/item/
---
## ConnectionParameterCollection indexer (1 of 2)

يسترجع عنصر [`ConnectionParameter`](../../connectionparameter/) في الفهرس المحدد.

```csharp
public ConnectionParameter this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // احصل على أول اتصال خارجي
                ExternalConnection connection = workbook.DataConnections[0];
                
                // احصل على مجموعة المعلمات
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // تحقق مما إذا كان هناك أي معلمات قبل الوصول
                if (parameters.Count > 0)
                {
                    // توضيح قراءة خاصية Item
                    ConnectionParameter firstParam = parameters[0];
                    Console.WriteLine($"Parameter type: {firstParam.GetType().Name}");
                }
                else
                {
                    Console.WriteLine("No parameters in collection");
                }
                
                // احفظ المصنف
                workbook.Save("ConnectionParameterItemDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ConnectionParameterCollection indexer (2 of 2)

يسترجع عنصر [`ConnectionParameter`](../../connectionparameter/) بالاسم المحدد.

```csharp
public ConnectionParameter this[string connParamName] { get; }
```

| معامل | الوصف |
| --- | --- |
| connParamName | اسم معلمة الاتصال |

### قيمة الإرجاع

العنصر بالاسم المحدد.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // احصل على أول اتصال خارجي
                ExternalConnection connection = workbook.DataConnections[0];
                
                // احصل على مجموعة المعلمات
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // تحقق مما إذا كانت هناك معلمات موجودة لتوضيح خاصية Item
                if (parameters.Count == 0)
                {
                    Console.WriteLine("No parameters in collection to demonstrate Item property");
                    return;
                }
                
                // احصل على اسم أول معلمة لاستخدامها في التوضيح
                string firstParamName = parameters[0].Name;
                
                // توضيح قراءة خاصية Item بالاسم
                ConnectionParameter retrievedParam = parameters[firstParamName];
                
                if (retrievedParam != null)
                {
                    Console.WriteLine($"Retrieved parameter name: {retrievedParam.Name}");
                }
                else
                {
                    Console.WriteLine("Parameter not found");
                }
                
                // احفظ المصنف
                workbook.Save("ConnectionParameterItemDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


