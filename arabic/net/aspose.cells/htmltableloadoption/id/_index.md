---
title: "HtmlTableLoadOption.Id"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlTableLoadOption. الحصول على أو تعيين معرف الجدول للاستيراد من HTML"
type: docs
url: /ar/net/aspose.cells/htmltableloadoption/id/
---
## HtmlTableLoadOption.Id property

احصل أو عيّن معرف الجدول لاستيراده من HTML

```csharp
public string Id { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyIdDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // تكوين خيارات تحميل الجدول
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1"; // Setting Id property
            tableLoadOption1.TargetSheetIndex = 0;
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2"; // Setting Id property
            tableLoadOption2.TargetSheetIndex = 0;

            // إضافة خيارات تحميل الجدول
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);

            // تحميل ملف HTML بالخيارات المحددة
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            Console.WriteLine("HTML tables with specified IDs have been loaded to Excel.");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


