---
title: "ExternalConnectionCollection.GetExternalConnectionById"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ExternalConnectionCollection. يسترجع عنصر ExternalConnection بالمعرف المحدد"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/
---
## ExternalConnectionCollection.GetExternalConnectionById method

يسترجع عنصر [`ExternalConnection`](../../externalconnection/) بالمعرف المحدد.

```csharp
public ExternalConnection GetExternalConnectionById(int connId)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| connId | Int32 | معرف الاتصال الخارجي |

### قيمة الإرجاع

العنصر بالمعرف المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionCollectionMethodGetExternalConnectionByIdWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع اتصالات بيانات تجريبية
            Workbook workbook = new Workbook();
            
            // احصل على مجموعة الاتصالات الخارجية
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // أنشئ وأضف الاتصالات باستخدام طرق API المناسبة
            // ملاحظة: في الاستخدام الفعلي، عادةً ما ستحصل على الاتصالات الموجودة
            // بدلاً من إنشاء جديدة بهذه الطريقة
            int connectionId1 = 1;
            int connectionId2 = 2;
            
            // احصل على اتصال محدد بالمعرف (سيكون فارغًا في البداية)
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(connectionId1);
            
            if (specificConn == null)
            {
                Console.WriteLine($"No connection found with ID {connectionId1}");
                // في الاستخدام الفعلي، ستعمل مع الاتصالات الموجودة
                // أو أنشئها عبر طرق API المناسبة
            }
            else
            {
                Console.WriteLine($"Found connection: ID={specificConn.ConnectionId}, Name={specificConn.Name}");
                specificConn.Name = "ModifiedConnection";
            }

            // احفظ المصنف
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


