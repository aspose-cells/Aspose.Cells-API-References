---
title: "ExternalConnection.IsNew"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. صحيحة إذا لم يتم تحديث الاتصال للمرة الأولى، وإلا خاطئة. يمكن أن يحدث هذا عندما يقوم المستخدم بحفظ الملف قبل أن تنتهي الاستعلام من الإرجاع"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/isnew/
---
## ExternalConnection.IsNew property

true إذا لم يتم تحديث الاتصال للمرة الأولى؛ وإلا false. يمكن أن يحدث هذا الحالة عندما يقوم المستخدم بحفظ الملف قبل أن ينتهي الاستعلام من الإرجاع.

```csharp
public bool IsNew { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsNewDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال خارجي (الاتصالات التي تم إنشاؤها حديثًا عادةً ما تكون \"IsNew\")
                ExternalConnection connection = workbook.DataConnections[0];
                
                // عرض قيمة IsNew الأولية
                Console.WriteLine("Initial IsNew value: " + connection.IsNew);
                
                // نظرًا لأن IsNew قابل للقراءة والكتابة، عرض تعيينه
                connection.IsNew = false;
                Console.WriteLine("Updated IsNew value: " + connection.IsNew);
                
                // حفظ المصنف مع إعدادات الاتصال المعدلة.
                workbook.Save("IsNewDemo.xlsx");
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


