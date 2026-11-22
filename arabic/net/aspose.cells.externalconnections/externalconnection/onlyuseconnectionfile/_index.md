---
title: "ExternalConnection.OnlyUseConnectionFile"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExternalConnection. تشير إلى ما إذا كان يجب على تطبيق الجداول الإلكترونية دائمًا واستخدام فقط معلومات الاتصال في ملف الاتصال الخارجي المشار إليه بصفة odcFile عند تحديث الاتصال. إذا كان false، يجب على التطبيق اتباع الإجراء المشار إليه بصفة reconnectionMethod."
type: docs
url: /ar/net/aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/
---
## ExternalConnection.OnlyUseConnectionFile property

يشير إلى ما إذا كان يجب على تطبيق الجدول الإلكتروني دائمًا واستخدام فقط معلومات الاتصال الموجودة في ملف الاتصال الخارجي المشار إليه بخصية odcFile عند تحديث الاتصال. إذا كان false، يجب على تطبيق الجدول الإلكتروني اتباع الإجراء المشار إليه بخصية reconnectionMethod.

```csharp
public bool OnlyUseConnectionFile { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOnlyUseConnectionFileDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال خارجي (على افتراض وجود واحد).
                ExternalConnection connection = workbook.DataConnections[0];
                
                // اعرض القيمة الحالية لـ OnlyUseConnectionFile
                Console.WriteLine("Initial OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // عيّن قيمة OnlyUseConnectionFile جديدة (نظرًا لأنها قراءة-كتابة)
                connection.OnlyUseConnectionFile = true;
                Console.WriteLine("Updated OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // بدّل القيمة لتوضيح إمكانية الإعداد
                connection.OnlyUseConnectionFile = !connection.OnlyUseConnectionFile;
                Console.WriteLine("Toggled OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // حفظ المصنف مع إعدادات الاتصال المعدلة.
                workbook.Save("OnlyUseConnectionFileDemo.xlsx");
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


