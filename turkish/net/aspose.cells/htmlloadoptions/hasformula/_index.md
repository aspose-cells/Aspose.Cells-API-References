---
title: "HtmlLoadOptions.HasFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlLoadOptions özelliği. Metnin, ... ile başlıyorsa formül olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/htmlloadoptions/hasformula/
---
## HtmlLoadOptions.HasFormula property

Metnin "=" ile başlıyorsa formül olup olmadığını gösterir.

```csharp
public bool HasFormula { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // HTML yükleme seçenekleri oluştur
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Formül dizgilerini düz metin olarak ele almak için HasFormula'ı false olarak ayarlayın
            loadOptions.HasFormula = false;
            
            // HTML dosyası ve yükleme seçenekleriyle bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // HTML içe aktarmayı göstermek için bazı hücre değerlerini görüntüle
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            
            // XLSX olarak kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


