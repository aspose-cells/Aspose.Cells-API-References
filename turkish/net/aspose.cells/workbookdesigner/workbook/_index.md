---
title: "WorkbookDesigner.Workbook"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookDesigner özelliği. Workbook nesnesini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/workbook/
---
## WorkbookDesigner.Workbook property

`Workbook` nesnesini alır ve ayarlar.

```csharp
public Workbook Workbook { get; set; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı tasarımcısı oluştur
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Workbook özelliğini yeni bir çalışma kitabı ile ayarla
            designer.Workbook = new Workbook();
            
            // Bir çalışma sayfası ve bazı şablon işaretçileri ekle
            Worksheet worksheet = designer.Workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&Person.Name");
            worksheet.Cells["B1"].PutValue("&Person.Age");

            // Veri kaynağı oluşturun
            List<Person1> persons = new List<Person1>
            {
                new Person1("John", 25),
                new Person1("Mary", 30)
            };

            // Veri kaynağını ayarlayın ve işleyin
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Sonuçları çıktı olarak ver
            Console.WriteLine("A2: " + worksheet.Cells["A2"].StringValue); // Should output "John"
            Console.WriteLine("B2: " + worksheet.Cells["B2"].IntValue);   // Should output 25
            Console.WriteLine("A3: " + worksheet.Cells["A3"].StringValue); // Should output "Mary"
            Console.WriteLine("B3: " + worksheet.Cells["B3"].IntValue);   // Should output 30

            // Çalışma kitabını kaydedin
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


