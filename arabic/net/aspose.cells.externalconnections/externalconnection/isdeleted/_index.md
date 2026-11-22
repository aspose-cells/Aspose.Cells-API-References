---
title: "ExternalConnection.IsDeleted"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تشير إلى ما إذا كان اتصال المصنف المرتبط قد تم حذفه. true إذا تم حذف الاتصال وإلا false"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/isdeleted/
---
## ExternalConnection.IsDeleted property

يشير إلى ما إذا تم حذف اتصال دفتر العمل المرتبط. true إذا تم حذف الاتصال؛ وإلا false.

```csharp
public bool IsDeleted { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال خارجي (على افتراض وجود واحد).
                ExternalConnection connection = workbook.DataConnections[0];
                
                // اعرض القيمة الأولية لـ IsDeleted
                Console.WriteLine("Initial IsDeleted value: " + connection.IsDeleted);
                
                // بدّل قيمة IsDeleted (نظرًا لأنه قابل للقراءة والكتابة)
                connection.IsDeleted = !connection.IsDeleted;
                Console.WriteLine("Updated IsDeleted value: " + connection.IsDeleted);
                
                // حفظ المصنف مع إعدادات الاتصال المعدلة.
                workbook.Save("IsDeletedDemo.xlsx");
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


