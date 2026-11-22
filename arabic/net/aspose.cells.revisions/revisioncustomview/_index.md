---
title: "الفئة RevisionCustomView"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Revisions.RevisionCustomView فئة. تمثل سجل مراجعة لإضافة أو إزالة عرض مخصص إلى دفتر العمل"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncustomview/
---
## RevisionCustomView class

يمثل سجل مراجعة لإضافة أو إزالة عرض مخصص إلى المصنف.

```csharp
public class RevisionCustomView : Revision
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncustomview/actiontype/) { get; } | يحصل على نوع الإجراء. |
| [Guid](../../aspose.cells.revisions/revisioncustomview/guid/) { get; } | يحصل على المعرف الفريد عالميًا للعرض المخصص. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | يحصل على رقم هذه المراجعة.(موروث من [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisioncustomview/type/) { get; } | يحصل على نوع المراجعة. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | يحصل على ورقة العمل. (موروث من [`Revision`](../revision/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCustomViewDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // أضف عرضًا مخصصًا لتوليد مراجعة محتملة
                // ملاحظة: استخدام CustomDocumentProperties كحل بديل لأن CustomViews غير متوفر
                workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");

                // الوصول إلى سجلات المراجعة (بافتراض وجودها)
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // اعرض الخصائص للقراءة فقط
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Action Type: {customViewRevision.ActionType}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");

                            // عرض الاستخدام الأساسي للخصائص
                            if (customViewRevision.Type == RevisionType.CustomView)
                            {
                                Console.WriteLine("This is a custom view revision.");
                            }

                            if (customViewRevision.ActionType == RevisionActionType.Add)
                            {
                                Console.WriteLine("The custom view was added.");
                            }
                            else if (customViewRevision.ActionType == RevisionActionType.Delete)
                            {
                                Console.WriteLine("The custom view was deleted.");
                            }
                        }
                    }
                }

                // احفظ المصنف
                workbook.Save("RevisionCustomViewDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


