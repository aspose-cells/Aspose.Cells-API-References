---
title: "WebQueryConnection.EditWebPage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebQueryConnection. عنوان URL لصفحة الويب التي يواجهها المستخدم وتظهر بيانات استعلام الويب. يتم حفظ هذا العنوان في حالة تم إعادة توجيه sourceDatatrue و url للإشارة إلى ملف XML. ثم يمكن عرض صفحة المستخدم في واجهة المستخدم ويمكن استرجاع بيانات XML في الخلفية"
type: docs
url: /ar/net/aspose.cells.externalconnections/webqueryconnection/editwebpage/
---
## WebQueryConnection.EditWebPage property

عنوان URL للصفحة الويب الموجهة للمستخدم والتي تعرض بيانات استعلام الويب. يتم حفظ هذا العنوان في الحالة التي تكون فيها sourceData="true" وتم إعادة توجيه url للإشارة إلى ملف XML. ثم يمكن عرض الصفحة الموجهة للمستخدم في واجهة المستخدم، ويمكن استرجاع بيانات XML خلف الكواليس.

```csharp
public string EditWebPage { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditWebPageDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // الوصول إلى أول اتصال استعلام ويب موجود (إن وجد)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // تعيين قيمة EditWebPage الأولية
                    connection.EditWebPage = "https://example.com/user-facing-page.html";
                    Console.WriteLine("Initial EditWebPage value: " + connection.EditWebPage);
                    
                    // تحديث قيمة EditWebPage
                    connection.EditWebPage = "https://example.com/updated-user-page.html";
                    Console.WriteLine("Updated EditWebPage value: " + connection.EditWebPage);
                    
                    // حفظ المصنف مع اتصال استعلام الويب
                    workbook.Save("WebQueryConnectionEditWebPageDemo.xlsx");
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


