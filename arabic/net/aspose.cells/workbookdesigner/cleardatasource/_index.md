---
title: "WorkbookDesigner.ClearDataSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorkbookDesigner. تمسح جميع مصادر البيانات"
type: docs
url: /ar/net/aspose.cells/workbookdesigner/cleardatasource/
---
## WorkbookDesigner.ClearDataSource method

يمسح جميع مصادر البيانات.

```csharp
public void ClearDataSource()
```

### أمثلة

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }

        public Person(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }

    public class WorkbookDesignerMethodClearDataSourceDemo
    {
        public static void Run()
        {
            WorkbookDesigner designer = new WorkbookDesigner();
            Worksheet worksheet = designer.Workbook.Worksheets[0];

            // إنشاء بيانات نموذجية
            List<Person> persons = new List<Person>
            {
                new Person("John", 30),
                new Person("Mary", 25),
                new Person("Peter", 35)
            };

            // إعداد العلامات الذكية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("&=Person.Name");
            worksheet.Cells["B2"].PutValue("&=Person.Age");

            // ربط البيانات الأول
            designer.SetDataSource("Person", persons);
            designer.Process();

            // مسح مصدر البيانات وإعادة الربط
            designer.ClearDataSource();
            designer.SetDataSource("Person", persons);
            designer.Process();

            // حفظ النتيجة
            designer.Workbook.Save("ClearedDataSourceOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


