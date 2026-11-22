---
title: "ExternalConnection.ConnectionId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تحدد المعرف الفريد لهذا الاتصال"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/connectionid/
---
## ExternalConnection.ConnectionId property

تحدد المعرف الفريد لهذا الاتصال.

```csharp
[Obsolete("Use ExternalConnection.Id property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ConnectionId { get; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية ExternalConnection.Id. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من أكتوبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyConnectionIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // الوصول إلى أول اتصال خارجي (المصنف يأتي باتصالات افتراضية)
                ExternalConnection connection = workbook.DataConnections[0];

                // اعرض قيمة ConnectionId (خاصية للقراءة فقط)
                Console.WriteLine("ConnectionId value: " + connection.ConnectionId);

                // اعرض قيمة Id للمقارنة (أيضًا للقراءة فقط)
                Console.WriteLine("Id value: " + connection.Id);

                // أظهر أن الخاصيتين للقراءة فقط بمحاولة عرضهما
                Console.WriteLine("ConnectionId and Id are both read-only properties");
                Console.WriteLine("ConnectionId: " + connection.ConnectionId + ", Id: " + connection.Id);

                // احفظ المصنف
                workbook.Save("ConnectionIdDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


