---
title: "ExternalConnection.SaveData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. صحيحة إذا كان يجب حفظ البيانات الخارجية التي تم جلبها عبر الاتصال لتعبئة جدول مع المصنف، وإلا خاطئة"
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/savedata/
---
## ExternalConnection.SaveData property

صحيح إذا كان يجب حفظ البيانات الخارجية التي تم جلبها عبر الاتصال لتعبئة جدول مع المصنف؛ وإلا، خطأ.

```csharp
public bool SaveData { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySaveDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال خارجي (على افتراض وجود واحد).
                ExternalConnection connection = workbook.DataConnections[0];
                
                // اعرض قيمة SaveData الحالية
                Console.WriteLine("Initial SaveData value: " + connection.SaveData);
                
                // إظهار تعيين الخاصية (نظرًا لأنها قابلة للقراءة والكتابة).
                connection.SaveData = !connection.SaveData;
                Console.WriteLine("Updated SaveData value: " + connection.SaveData);
                
                // حفظ المصنف مع إعدادات الاتصال المعدلة.
                workbook.Save("SaveDataDemo.xlsx");
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


