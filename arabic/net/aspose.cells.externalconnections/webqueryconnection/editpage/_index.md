---
title: "WebQueryConnection.EditPage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. عنوان URL لصفحة الويب التي يواجهها المستخدم وتظهر بيانات استعلام الويب. يتم حفظ هذا العنوان في حالة تم إعادة توجيه sourceDatatrue و url للإشارة إلى ملف XML. ثم يمكن عرض صفحة المستخدم في واجهة المستخدم ويمكن استرجاع بيانات XML في الخلفية"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/editpage/
---
## WebQueryConnection.EditPage property

عنوان URL للصفحة الويب الموجهة للمستخدم والتي تعرض بيانات استعلام الويب. يتم حفظ هذا العنوان في الحالة التي تكون فيها sourceData="true" وتم إعادة توجيه url للإشارة إلى ملف XML. ثم يمكن عرض الصفحة الموجهة للمستخدم في واجهة المستخدم، ويمكن استرجاع بيانات XML خلف الكواليس.

```csharp
[Obsolete("Use WebQueryConnection.EditWebPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EditPage { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية WebQueryConnection.EditWebPage. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2017. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditPageDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال استعلام ويب موجود إذا كان متاحًا
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // عرض قيمة EditPage الأولية
                    Console.WriteLine("Initial EditPage value: " + connection.EditPage);
                    
                    // تعيين EditPage إلى عنوان URL جديد (نظرًا لأنه قابل للقراءة والكتابة)
                    connection.EditPage = "https://example.com/editpage";
                    Console.WriteLine("Updated EditPage value: " + connection.EditPage);
                    
                    // احفظ المصنف
                    workbook.Save("WebQueryConnectionEditPageDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
                }
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


