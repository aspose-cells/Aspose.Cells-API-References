---
title: "الفئة RevisionDefinedName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Revisions.RevisionDefinedName. تمثل سجل مراجعة لتغيير اسم معرف"
type: docs
url: /ar/net/aspose.cells.revisions/revisiondefinedname/
---
## RevisionDefinedName class

يمثل سجل مراجعة لتغيير اسم معرف.

```csharp
public class RevisionDefinedName : Revision
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | يحصل على رقم هذه المراجعة.(موروث من [`Revision`](../revision/).) |
| [NewFormula](../../aspose.cells.revisions/revisiondefinedname/newformula/) { get; } | يحصل على الصيغة. |
| [OldFormula](../../aspose.cells.revisions/revisiondefinedname/oldformula/) { get; } | يحصل على الصيغة القديمة. |
| [Text](../../aspose.cells.revisions/revisiondefinedname/text/) { get; } | يحصل على نص الاسم المعرف. |
| override [Type](../../aspose.cells.revisions/revisiondefinedname/type/) { get; } | يمثل نوع المراجعة. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | يحصل على ورقة العمل. (موروث من [`Revision`](../revision/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDefinedNameDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // إضافة اسم معرف إلى المصنف
                int nameIndex = workbook.Worksheets.Names.Add("TestDefinedName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // تعديل الاسم المعرف لإنشاء مراجعة
                definedName.RefersTo = "=Sheet1!$B$1";

                // حفظ المصنف لإنشاء سجلات المراجعة
                string filePath = "RevisionDefinedNameDemo.xlsx";
                workbook.Save(filePath);

                // إعادة فتح المصنف للوصول إلى معلومات المراجعة
                Workbook revisionWorkbook = new Workbook(filePath);

                // التكرار عبر سجلات المراجعة للعثور على إدخالات RevisionDefinedName
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;

                            // عرض خصائص RevisionDefinedName
                            Console.WriteLine($"Revision Type: {revisionDefinedName.Type}");
                            Console.WriteLine($"Defined Name Text: {revisionDefinedName.Text}");
                            Console.WriteLine($"Old Formula: {revisionDefinedName.OldFormula}");
                            Console.WriteLine($"New Formula: {revisionDefinedName.NewFormula}");
                        }
                    }
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


