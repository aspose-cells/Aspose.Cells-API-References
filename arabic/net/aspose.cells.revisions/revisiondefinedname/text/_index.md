---
title: "RevisionDefinedName.Text"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionDefinedName. تحصل على نص الاسم المحدد"
type: docs
url: /ar/net/aspose.cells.revisions/revisiondefinedname/text/
---
## RevisionDefinedName.Text property

يحصل على نص الاسم المعرف.

```csharp
public string Text { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionDefinedNamePropertyTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء اسم محدد
            int index = workbook.Worksheets.Names.Add("TestName");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1";
            
            // تعديل الاسم المحدد لتوليد مراجعة
            name.RefersTo = "=Sheet1!$B$1";
            
            // احفظ إلى ملف لتوليد مراجعات
            workbook.Save("RevisionDefinedName.xlsx");
            
            // أعد فتح الملف لقراءة المراجعات
            Workbook revisionWorkbook = new Workbook("RevisionDefinedName.xlsx");
            
            // تحقق من المراجعات
            foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.DefinedName)
                    {
                        RevisionDefinedName rdn = (RevisionDefinedName)rv;
                        Console.WriteLine("Defined Name Text: " + rdn.Text);
                        Console.WriteLine("Old Formula: " + rdn.OldFormula);
                        Console.WriteLine("New Formula: " + rdn.NewFormula);
                    }
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


