---
title: "ExternalConnection.SSOId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. معرف لتقنية الدخول الأحادي SSO المستخدمة للمصادقة بين خادم spreadsheetML الوسيط ومصدر البيانات الخارجي"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/ssoid/
---
## ExternalConnection.SSOId property

معرّف لتقنية الدخول الموحد (Single Sign On (SSO)) المستخدمة للمصادقة بين خادم spreadsheetML وسيط ومصدر البيانات الخارجي.

```csharp
public string SSOId { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySSOIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال خارجي
                ExternalConnection connection = workbook.DataConnections[0];
                
                // عرض قيمة SSOId الأولية (من المحتمل أن تكون فارغة للاتصال الجديد)
                Console.WriteLine("Initial SSOId value: " + connection.SSOId);
                
                // تعيين قيمة SSOId جديدة (نظرًا لأنها قابلة للقراءة والكتابة)
                connection.SSOId = "sso-12345";
                Console.WriteLine("Updated SSOId value: " + connection.SSOId);
                
                // مسح SSOId
                connection.SSOId = null;
                Console.WriteLine("Cleared SSOId value: " + connection.SSOId);
                
                // حفظ المصنف مع إعدادات الاتصال المعدلة.
                workbook.Save("SSOIdDemo.xlsx");
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


