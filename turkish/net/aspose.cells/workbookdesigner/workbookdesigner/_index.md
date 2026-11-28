---
title: "WorkbookDesigner.WorkbookDesigner"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookDesigner yapıcı. WorkbookDesigner sınıfının yeni bir örneğini başlatır"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/workbookdesigner/
---
## WorkbookDesigner() {#constructor}

Yeni bir [`WorkbookDesigner`](../) sınıfının bir örneğini başlatır.

```csharp
public WorkbookDesigner()
```

### Örnekler

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
            // Yapıcıyı kullanarak yeni bir WorkbookDesigner oluşturun
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // Örnek veri kaynağı oluşturun
            List<Level> levels = new List<Level>();
            levels.Add(new Level("r1", "c1"));
            levels.Add(new Level("r2", "c2"));
            levels.Add(new Level("r3", "c3"));

            // Yeni bir çalışma kitabı oluşturun ve bunu tasarımcının çalışma kitabı olarak ayarlayın
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına işaretçileri ayarlayın
            worksheet.Cells["A1"].PutValue("&Level.Name");
            worksheet.Cells["B1"].PutValue("&Level.Value");

            // Çalışma kitabını tasarımcıya ayarlayın
            designer.Workbook = workbook;

            // Veri kaynağını ayarlayın ve işleyin
            designer.SetDataSource("Level", levels);
            designer.Process();

            // Sonucu kaydet
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

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner(Workbook) {#constructor_1}

Yeni bir [`WorkbookDesigner`](../) sınıfının bir örneğini başlatır.

```csharp
public WorkbookDesigner(Workbook workbook)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| çalışma kitabı | Çalışma Kitabı | Şablon çalışma kitabı dosyası. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodCtorWithWorkbookDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelerde örnek veri ayarlayın
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("&=$ds.object.object1.name");
            
            // JSON veri kaynağı oluştur
            string jsonData = "{\"object\": {\"object1\": {\"name\": \"John Doe\"}}}";
            
            // WorkbookDesigner'ı çalışma kitabı ile başlatın
            WorkbookDesigner designer = new WorkbookDesigner(workbook);
            
            // JSON veri kaynağını ayarlayın
            designer.SetJsonDataSource("ds", jsonData);
            
            // Tasarımcıyı işleyin
            designer.Process();
            
            // Sonucu çıktı olarak ver
            Console.WriteLine("Processed value: " + worksheet.Cells["A2"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


