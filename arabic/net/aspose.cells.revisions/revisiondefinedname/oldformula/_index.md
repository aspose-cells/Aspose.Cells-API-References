---
title: "RevisionInsertSheet.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionInsertSheet. تحصل على اسم ورقة العمل"
type: docs
url: /ar/net/aspose.cells.revisions/revisiondefinedname/oldformula/
---
## RevisionDefinedName.OldFormula property

يحصل على الصيغة القديمة.

```csharp
public string OldFormula { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionDefinedNamePropertyOldFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // أضف اسمًا محددًا لتوليد تاريخ المراجعة
                int nameIndex = workbook.Worksheets.Names.Add("SampleName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // تعديل الاسم المعرف لإنشاء مراجعة
                definedName.RefersTo = "=Sheet1!$B$1";

                // احفظ المصنف لاستمرار المراجعات
                string filePath = "OldFormulaDemo.xlsx";
                workbook.Save(filePath);

                // أعد فتح دفتر العمل للوصول إلى سجلات المراجعات
                Workbook revisionWorkbook = new Workbook(filePath);

                // تكرّر عبر سجلات المراجعة للعثور على مراجعات الأسماء المحددة
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;
                            Console.WriteLine("Defined Name Text: " + revisionDefinedName.Text);
                            Console.WriteLine("Old Formula: " + revisionDefinedName.OldFormula);
                            Console.WriteLine("New Formula: " + revisionDefinedName.NewFormula);
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

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


