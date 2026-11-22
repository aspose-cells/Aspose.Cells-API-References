---
title: "HtmlLoadOptions.TableLoadOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlLoadOptions. الحصول على كائن HtmlTableLoadOptionCollection"
type: docs
url: /ar/net/aspose.cells/htmlloadoptions/tableloadoptions/
---
## HtmlLoadOptions.TableLoadOptions property

احصل على مثيل HtmlTableLoadOptionCollection

```csharp
public HtmlTableLoadOptionCollection TableLoadOptions { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyTableLoadOptionsDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            
            // إضافة خيارات تحميل الجدول حسب الفهرس
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            
            // إضافة خيارات تحميل الجدول حسب المعرف
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table2";
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // تحميل ملف HTML باستخدام الخيارات
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // حفظ الناتج
            workbook.Save("output.xlsx");
            
            // مسح وإضافة خيارات تحميل جدول جديدة
            loadOptions.TableLoadOptions.Clear();
            
            // إضافة خيارات تحميل الجدول مع تعيين فهرس الورقة
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 -> Sheet 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 -> Sheet 0
            
            // إضافة خيارات تحميل الجدول مع المعرف وتعيين الورقة
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "mainTable";
            tableLoadOption.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            // تحميل وحفظ مرة أخرى مع خيارات جديدة
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output_mapped.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOptionCollection](../../htmltableloadoptioncollection/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


