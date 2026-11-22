---
title: "ExternalConnection.Credentials"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تحدد طريقة المصادقة التي يجب استخدامها عند إنشاء أو إعادة إنشاء الاتصال."
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/credentials/
---
## ExternalConnection.Credentials property

يحدد طريقة المصادقة التي يجب استخدامها عند إنشاء (أو إعادة إنشاء) الاتصال.

```csharp
[Obsolete("Use ExternalConnection.CredentialsMethodType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CredentialsMethodType Credentials { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية ExternalConnection.CredentialsMethodType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2017. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyCredentialsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال خارجي (على افتراض وجود واحد).
                ExternalConnection connection = workbook.DataConnections[0];
                
                // اعرض قيمة Credentials الحالية
                Console.WriteLine("Initial Credentials value: " + connection.Credentials);
                
                // حدد قيمة Credentials جديدة (نظرًا لأنها قابلة للقراءة والكتابة)
                connection.Credentials = CredentialsMethodType.Integrated;
                Console.WriteLine("Updated Credentials value: " + connection.Credentials);
                
                // تجول عبر القيم الممكنة
                foreach (CredentialsMethodType method in Enum.GetValues(typeof(CredentialsMethodType)))
                {
                    connection.Credentials = method;
                    Console.WriteLine($"Credentials set to: {method}");
                }
                
                // حفظ المصنف مع إعدادات الاتصال المعدلة.
                workbook.Save("CredentialsDemo.xlsx");
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

* enum [CredentialsMethodType](../../credentialsmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


