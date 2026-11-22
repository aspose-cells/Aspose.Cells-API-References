---
title: "WorkbookDesigner.Workbook"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookDesigner. تحصل وتضبط كائن Workbook"
type: docs
url: /ar/net/aspose.cells/workbookdesigner/workbook/
---
## WorkbookDesigner.Workbook property

تحصل وتضبط كائن `Workbook`.

```csharp
public Workbook Workbook { get; set; }
```

### أمثلة

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Person1
    {
        public string Name { get; set; }
        public int Age { get; set; }

        public Person1(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }

    public class WorkbookDesignerPropertyWorkbookDemo
    {
        public static void Run()
        {
            // إنشاء مصمم دفتر عمل جديد
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // ضبط خاصية دفتر العمل بدفتر عمل جديد
            designer.Workbook = new Workbook();
            
            // إضافة ورقة عمل وبعض علامات القالب
            Worksheet worksheet = designer.Workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&Person.Name");
            worksheet.Cells["B1"].PutValue("&Person.Age");

            // إنشاء مصدر بيانات
            List<Person1> persons = new List<Person1>
            {
                new Person1("John", 25),
                new Person1("Mary", 30)
            };

            // تعيين مصدر البيانات ومعالجته
            designer.SetDataSource("Person", persons);
            designer.Process();

            // إخراج النتائج
            Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // Should output "John"
            Console.WriteLine("B2: " + worksheet.Cells["B2"].IntValue);   // Should output 25
            Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // Should output "Mary"
            Console.WriteLine("B3: " + worksheet.Cells["B3"].IntValue);   // Should output 30

            // احفظ المصنف
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


