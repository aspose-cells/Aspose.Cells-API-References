---
title: "RevisionHeader.UserName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionHeader. تحصل وتضبط اسم المستخدم الذي يجري المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisionheader/username/
---
## RevisionHeader.UserName property

يحصل ويضبط اسم المستخدم الذي يقوم بالمراجعة.

```csharp
public string UserName { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertyUserNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            try
            {
                // أنشئ مثيلًا لـ RevisionHeader
                RevisionHeader revisionHeader = new RevisionHeader();

                // عيّن خاصية UserName
                revisionHeader.UserName = "JohnDoe";

                // اعرض القيمة الحالية لخاصية UserName
                Console.WriteLine("UserName value: " + revisionHeader.UserName);

                // عدّل خاصية UserName
                revisionHeader.UserName = "JaneSmith";
                Console.WriteLine("Modified UserName value: " + revisionHeader.UserName);

                // احفظ workbook لتوضيح أن الخاصية تُستخدم
                workbook.Save("UserNameDemo.xlsx");
                Console.WriteLine("UserName property has been demonstrated and workbook saved.");
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

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


