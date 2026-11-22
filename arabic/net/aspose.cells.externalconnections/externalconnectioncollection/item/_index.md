---
title: "ExternalConnectionCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnectionCollection. تحصل على عنصر ExternalConnection في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnectioncollection/item/
---
## ExternalConnectionCollection indexer (1 of 2)

يحصل على العنصر [`ExternalConnection`](../../externalconnection/) في الفهرس المحدد.

```csharp
public ExternalConnection this[int index] { get; }
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

    public class ExternalConnectionCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // الوصول إلى مجموعة الاتصالات الخارجية
                ExternalConnectionCollection connections = workbook.DataConnections;

                // تحقق مما إذا كان هناك أي اتصالات
                if (connections.Count > 0)
                {
                    // عرض كيفية الوصول إلى عنصر عبر الفهرس (عملية قراءة)
                    ExternalConnection connection = connections[0];

                    // عرض معلومات الاتصال
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                    Console.WriteLine($"Connection ID: {connection.ConnectionId}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }

                // احفظ المصنف
                workbook.Save("ExternalConnectionItemDemo.xlsx");
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

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ExternalConnectionCollection indexer (2 of 2)

يحصل على العنصر [`ExternalConnection`](../../externalconnection/) بالاسم المحدد.

```csharp
public ExternalConnection this[string connectionName] { get; }
```

| معامل | الوصف |
| --- | --- |
| connectionName | اسم اتصال البيانات |

### قيمة الإرجاع

العنصر بالاسم المحدد.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى مجموعة الاتصالات الخارجية
                ExternalConnectionCollection connections = workbook.DataConnections;
                
                // أضف اتصالًا تجريبيًا (إذا لزم الأمر للعرض)
                // يفترض ذلك أن المجموعة تسمح بإضافة الاتصالات
                // connections.Add(new ExternalConnection());
                
                // عرض كيفية الوصول إلى عنصر بالاسم (عملية قراءة)
                // ملاحظة: في سيناريو واقعي، ستحتاج إلى أسماء اتصالات فعلية
                if (connections.Count > 0)
                {
                    // احصل على اسم أول اتصال (إن وجد)
                    string connectionName = connections[0].Name;
                    
                    // الوصول إلى خاصية Item
                    ExternalConnection connection = connections[connectionName];
                    
                    // عرض معلومات الاتصال
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }
                
                // احفظ المصنف
                workbook.Save("ExternalConnectionDemo.xlsx");
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

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


