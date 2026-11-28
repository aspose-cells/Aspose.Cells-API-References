---
title: "MarkdownSaveOptions.CalculateFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MarkdownSaveOptions özelliği. Markdown dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/markdownsaveoptions/calculateformula/
---
## MarkdownSaveOptions.CalculateFormula property

Markdown dosyası kaydedilmeden önce formüllerin hesaplanıp hesaplanmayacağını gösterir.

```csharp
public bool CalculateFormula { get; set; }
```

### Açıklamalar

Varsayılan değer false'tur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Formüller içeren örnek veri ekle
            worksheet.Cells["A1"].PutValue("Price");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].Formula = "=A2*B2";

            try
            {
                // MarkdownSaveOptions örneği oluştur
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // CalculateFormula'ın varsayılan değerini göster
                Console.WriteLine("Default CalculateFormula value: " + saveOptions.CalculateFormula);

                // Kaydetmeden önce formülleri hesaplamak için CalculateFormula'ı true olarak ayarla
                saveOptions.CalculateFormula = true;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Formül hesaplaması etkinleştirilmiş şekilde çalışma kitabını kaydet
                workbook.Save("CalculateFormula_Enabled.md", saveOptions);

                // Formülleri olduğu gibi kaydetmek için CalculateFormula'ı false olarak ayarla
                saveOptions.CalculateFormula = false;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Formül hesaplaması devre dışı bırakılmış şekilde çalışma kitabını kaydet
                workbook.Save("CalculateFormula_Disabled.md", saveOptions);

                Console.WriteLine("CalculateFormula demonstration completed successfully.");
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

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


