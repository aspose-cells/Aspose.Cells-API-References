---
title: "Name.Text"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Name özelliği. Nesnenin ad metnini alır"
type: docs
url: /tr/net/aspose.cells/name/text/
---
## Name.Text property

Nesnenin ad metnini alır.

```csharp
public string Text { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Adlandırılmış bir aralık oluştur
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // Text özelliğini ayarlayın ve görüntüleyin
            namedRange.Text = "MyCustomName";
            Console.WriteLine("Named range text: " + namedRange.Text);
            
            // Çalışma kitabını kaydedin
            workbook.Save("NamedRangeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


