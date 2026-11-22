---
title: "ExternalConnection.SavePassword"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. True إذا كان يجب حفظ كلمة المرور كجزء من سلسلة الاتصال وإلا False"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/savepassword/
---
## ExternalConnection.SavePassword property

صحيح إذا كان يجب حفظ كلمة المرور كجزء من سلسلة الاتصال؛ وإلا، خطأ.

```csharp
public bool SavePassword { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySavePasswordDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // الوصول إلى أول اتصال خارجي (على افتراض وجود واحد).
                ExternalConnection connection = workbook.DataConnections[0];

                // اعرض القيمة الحالية لـ SavePassword
                Console.WriteLine("Initial SavePassword value: " + connection.SavePassword);

                // إظهار تعيين الخاصية (نظرًا لأنها قابلة للقراءة والكتابة).
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Updated SavePassword value: " + connection.SavePassword);

                // بدّل القيمة لتوضيح إمكانية الإعداد
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Toggled SavePassword value: " + connection.SavePassword);

                // حفظ المصنف مع إعدادات الاتصال المعدلة.
                workbook.Save("SavePasswordDemo.xlsx");
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


