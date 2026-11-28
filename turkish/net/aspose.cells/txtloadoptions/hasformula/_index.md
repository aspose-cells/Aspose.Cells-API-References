---
title: "TxtLoadOptions.HasFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions özelliği. Metnin formül olup olmadığını, belirli bir karakterle başlıyorsa gösterir"
type: docs
url: /tr/net/aspose.cells/txtloadoptions/hasformula/
---
## TxtLoadOptions.HasFormula property

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
    public class TxtLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // Metin yükleme seçeneklerini oluşturun ve formül ayrıştırmayı etkinleştirin
            TxtLoadOptions options = new TxtLoadOptions();
            options.HasFormula = true;
            options.SeparatorString = "|";

            // Metin dosyasındaki formüllerle çalışma kitabını yükleyin
            Workbook workbook = new Workbook("example.csv", options);
            
            // Formül içeren bir hücreye erişin ve görüntüleyin
            Console.WriteLine("Cell K2 formula: " + workbook.Worksheets[0].Cells["K2"].Formula);
            
            // Çalışma kitabını kaydedin
            workbook.Save("example_output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


