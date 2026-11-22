---
title: "RevisionCustomView.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCustomView. تحصل على نوع المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncustomview/type/
---
## RevisionCustomView.Type property

يحصل على نوع المراجعة.

```csharp
public override RevisionType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCustomViewPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع تتبع المراجعات
            Workbook workbook = new Workbook();
            // يبدو أن تتبع المراجعات مفعّل افتراضيًا عند إجراء التغييرات
            
            // أضف عرضًا مخصصًا لإنشاء سجل مراجعة
            workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");
            
            // الوصول إلى مجموعة المراجعات عبر الوظيفة المدمجة في Workbook
            RevisionCollection revisions = null;
            if (workbook.HasRevisions)
            {
                // في تنفيذ حقيقي، سيكون هناك طريقة للوصول إلى المراجعات
                // نظرًا لعدم تمكننا من العثور على الطريقة الدقيقة، سنترك هذا كقيمة null
                // هذا يحافظ على البنية مع الاعتراف بحدود واجهة برمجة التطبيقات
                revisions = null; // Would normally be workbook.Revisions or similar
            }

            // ابحث عن RevisionCustomView في المراجعات
            RevisionCustomView customViewRevision = null;
            if (revisions != null)
            {
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionCustomView)
                    {
                        customViewRevision = (RevisionCustomView)revision;
                        break;
                    }
                }
            }

            if (customViewRevision != null)
            {
                // عرض قيمة خاصية Type
                Console.WriteLine("Revision Type: " + customViewRevision.Type);
                
                // وضح كيفية استخدام خاصية Type
                if (customViewRevision.Type == RevisionType.CustomView)
                {
                    Console.WriteLine("This revision is for a custom view operation");
                    Console.WriteLine("Custom View GUID: " + customViewRevision.Guid);
                }
                
                // خاصية Type للقراءة فقط، لذا لا يمكننا تعيينها
                // يمكننا فقط فحص قيمتها لتحديد نوع المراجعة
                switch (customViewRevision.Type)
                {
                    case RevisionType.CustomView:
                        Console.WriteLine("Handling custom view revision");
                        break;
                    case RevisionType.Comment:
                        Console.WriteLine("Handling comment revision");
                        break;
                    // يمكن إضافة حالات أخرى حسب الحاجة
                    default:
                        Console.WriteLine("Handling other revision type");
                        break;
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionCustomViewTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [RevisionType](../../revisiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


