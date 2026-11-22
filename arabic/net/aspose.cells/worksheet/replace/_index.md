---
title: "Worksheet.Replace"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تستبدل جميع نصوص الخلايا بسلسلة جديدة"
type: docs
url: /ar/net/aspose.cells/worksheet/replace/
---
## Worksheet.Replace method

يستبدل نص جميع الخلايا بسلسلة جديدة.

```csharp
public int Replace(string oldString, string newString)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| oldString | String | قيمة السلسلة القديمة. |
| newString | String | قيمة السلسلة الجديدة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("Hello Aspose");
            worksheet.Cells["A3"].PutValue("Hello Cells");
            
            // إضافة مربع نص مع نص تجريبي
            worksheet.TextBoxes.Add(5, 0, 100, 50);
            worksheet.TextBoxes[0].Text = "Hello TextBox";
            
            // تعيين الترويسة والتذييل
            worksheet.PageSetup.SetHeader(0, "Hello Header");
            worksheet.PageSetup.SetFooter(0, "Hello Footer");
            
            // استبدل "Hello" بـ "Hi" في جميع المحتويات
            string findText = "Hello";
            string replaceText = "Hi";
            worksheet.Replace(findText, replaceText);
            
            // استبدال في رؤوس/تذييلات
            for (int i = 0; i < 3; i++)
            {
                if (worksheet.PageSetup.GetHeader(i) != null)
                    worksheet.PageSetup.SetHeader(i, worksheet.PageSetup.GetHeader(i).Replace(findText, replaceText));
                
                if (worksheet.PageSetup.GetFooter(i) != null)
                    worksheet.PageSetup.SetFooter(i, worksheet.PageSetup.GetFooter(i).Replace(findText, replaceText));
            }
            
            // استبدال في مربعات النص
            foreach (Aspose.Cells.Drawing.TextBox textBox in worksheet.TextBoxes)
            {
                if (textBox.Text != null)
                {
                    textBox.Text = textBox.Text.Replace(findText, replaceText);
                }
            }
            
            // احفظ المصنف
            workbook.Save("ReplaceDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


