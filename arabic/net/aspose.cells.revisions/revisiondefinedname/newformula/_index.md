---
title: "RevisionDefinedName.NewFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionDefinedName. تحصل على الصيغة"
type: docs
url: /ar/net/aspose.cells.revisions/revisiondefinedname/newformula/
---
## RevisionDefinedName.NewFormula property

يحصل على الصيغة.

```csharp
public string NewFormula { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionDefinedNamePropertyNewFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء مصنف جديد وإضافة بعض البيانات
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].Value = "Initial";

                // أضف اسمًا معرفًا يشير إلى A1
                int nameIdx = workbook.Worksheets.Names.Add("DemoName");
                Name definedName = workbook.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // غيّر الاسم المحدد لتوليد مراجعة (الآن يشير إلى B1)
                definedName.RefersTo = "=Sheet1!$B$1";

                // احفظ المصنف لتضمين معلومات المراجعة
                string fileName = "RevisionDefinedName_NewFormulaDemo.xlsx";
                workbook.Save(fileName);

                // أعد فتح المصنف لقراءة سجلات المراجعة
                Workbook revWorkbook = new Workbook(fileName);

                // تكرّر عبر المراجعات وعرض NewFormula
                foreach (RevisionLog log in revWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rev in log.Revisions)
                    {
                        if (rev.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName rdn = (RevisionDefinedName)rev;
                            Console.WriteLine($"Defined Name Text: {rdn.Text}");
                            Console.WriteLine($"Old Formula: {rdn.OldFormula}");
                            Console.WriteLine($"New Formula: {rdn.NewFormula}");
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


