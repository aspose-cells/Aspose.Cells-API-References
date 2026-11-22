---
title: "Name.FullText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Name. يحصل على النص الكامل للاسم للكائن مع إعداد النطاق"
type: docs
url: /ar/net/aspose.cells/name/fulltext/
---
## Name.FullText property

يحصل على النص الكامل لاسم الكائن مع إعداد النطاق.

```csharp
public string FullText { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyFullTextDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء بعض النطاقات المسمّاة
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells.CreateRange("A1", "B5").Name = "TestRange1";
            worksheet.Cells.CreateRange("C1", "D5").Name = "TestRange2";
            
            // احصل على مجموعة الأسماء
            NameCollection names = workbook.Worksheets.Names;
            
            // ابحث عن اسم باستخدام FullText
            string reference = "=Sheet1!$A$1:$B$5";
            Name foundName = FindNameByFullText(names, reference);
            
            // إخراج النتائج
            if (foundName != null)
            {
                Console.WriteLine("Found name: " + foundName.Text);
                Console.WriteLine("FullText: " + foundName.FullText);
            }
            else
            {
                Console.WriteLine("Name not found");
            }
        }
        
        public static Name FindNameByFullText(NameCollection names, string reference)
        {
            if (reference.IndexOf('=') == 0)
            {
                reference = reference.Substring(1);
            }
            foreach (Name nm in names)
            {
                if (nm.FullText.Equals(reference))
                {
                    return nm;
                }
            }
            return null;
        }
    }
}
```

### انظر أيضًا

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


