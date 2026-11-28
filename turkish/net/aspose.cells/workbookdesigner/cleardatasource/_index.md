---
title: "WorkbookDesigner.ClearDataSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookDesigner yöntemi. Tüm veri kaynaklarını temizler"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/cleardatasource/
---
## WorkbookDesigner.ClearDataSource method

Tüm veri kaynaklarını temizler.

```csharp
public void ClearDataSource()
```

### Örnekler

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

            // Örnek veri oluştur
            List<Person> persons = new List<Person>
            {
                new Person("John", 30),
                new Person("Mary", 25),
                new Person("Peter", 35)
            };

            // Akıllı işaretçileri ayarlayın
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("&=Person.Name");
            worksheet.Cells["B2"].PutValue("&=Person.Age");

            // İlk veri bağlama
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Veri kaynağını temizle ve yeniden bağla
            designer.ClearDataSource();
            designer.SetDataSource("Person", persons);
            designer.Process();

            // Sonucu kaydet
            designer.Workbook.Save("ClearedDataSourceOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


