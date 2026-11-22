---
title: "WorkbookDesigner.WorkbookDesigner"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ WorkbookDesigner. يهيئ مثيلًا جديدًا من فئة WorkbookDesigner"
type: docs
url: /ar/net/aspose.cells/workbookdesigner/workbookdesigner/
---
## WorkbookDesigner() {#constructor}

يُنشئ مثيلًا جديدًا من الفئة [`WorkbookDesigner`](../).

```csharp
public WorkbookDesigner()
```

### أمثلة

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء WorkbookDesigner جديد باستخدام المُنشئ
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // إنشاء مصدر بيانات تجريبي
            List<Level> levels = new List<Level>();
            levels.Add(new Level("r1", "c1"));
            levels.Add(new Level("r2", "c2"));
            levels.Add(new Level("r3", "c3"));

            // إنشاء مصنف جديد وتعيينه كمصنف للمصمم
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين العلامات في ورقة العمل
            worksheet.Cells["A1"].PutValue("&Level.Name");
            worksheet.Cells["B1"].PutValue("&Level.Value");

            // تعيين المصنف للمصمم
            designer.Workbook = workbook;

            // تعيين مصدر البيانات ومعالجته
            designer.SetDataSource("Level", levels);
            designer.Process();

            // حفظ النتيجة
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }

    public class Level
    {
        public string Name { get; set; }
        public string Value { get; set; }

        public Level(string name, string value)
        {
            Name = name;
            Value = value;
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner(Workbook) {#constructor_1}

يُنشئ مثيلًا جديدًا من الفئة [`WorkbookDesigner`](../).

```csharp
public WorkbookDesigner(Workbook workbook)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| المصنف | المصنف | ملف مصنف القالب. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodCtorWithWorkbookDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين بيانات تجريبية في الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("&=$ds.object.object1.name");
            
            // إنشاء مصدر بيانات JSON
            string jsonData = "{\"object\": {\"object1\": {\"name\": \"John Doe\"}}}";
            
            // تهيئة WorkbookDesigner بالمصنف
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            
            // تعيين مصدر بيانات JSON
            designer.SetJsonDataSource("ds", jsonData);
            
            // معالجة المصمم
            designer.Process();
            
            // أخرج النتيجة.
            Console.WriteLine("Processed value: " + worksheet.Cells["A2"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


