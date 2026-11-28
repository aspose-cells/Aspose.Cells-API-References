---
title: "MarkdownLoadOptions.HasFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MarkdownLoadOptions özelliği. Metnin formül olup olmadığını, belirli bir karakterle başlayıp başlamadığına göre gösterir"
type: docs
url: /tr/net/aspose.cells/markdownloadoptions/hasformula/
---
## MarkdownLoadOptions.HasFormula property

Metnin "=" ile başlıyorsa formül olup olmadığını gösterir.

```csharp
public bool HasFormula { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // MarkdownLoadOptions örneği oluştur
                MarkdownLoadOptions options = new MarkdownLoadOptions();

                // HasFormula varsayılan değerini göster
                Console.WriteLine($"Default HasFormula value: {options.HasFormula}");

                // HasFormula değerini true olarak ayarla
                options.HasFormula = true;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // HasFormula değerini false olarak ayarla
                options.HasFormula = false;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Örnek markdown içeriğiyle bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();

                // Seçeneklerin kullanılabileceğini göstermek için çalışma kitabını kaydet
                workbook.Save("HasFormulaDemo.xlsx");

                Console.WriteLine("HasFormula property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [MarkdownLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


