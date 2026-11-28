---
title: "LoadOptions.ParsingFormulaOnOpen"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Dosya okunurken formülün ayrıştırılıp ayrıştırılmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/loadoptions/parsingformulaonopen/
---
## LoadOptions.ParsingFormulaOnOpen property

Dosya okunurken formülün ayrıştırılıp ayrıştırılmayacağını gösterir.

```csharp
public bool ParsingFormulaOnOpen { get; set; }
```

### Açıklamalar

Yalnızca Excel Xlsx, Xltx, Xltm ve Xlsm dosyaları için geçerlidir çünkü dosyalardaki formüller dize formülü olarak depolanır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingFormulaOnOpenDemo
    {
        public static void Run()
        {
            // Yükleme seçenekleri oluştur
            LoadOptions loadOptions = new LoadOptions();
            
            // Yükleme sırasında formül ayrıştırmayı atlamak için ParsingFormulaOnOpen'ı false olarak ayarla
            loadOptions.ParsingFormulaOnOpen = false;
            
            // Belirtilen seçeneklerle çalışma kitabını yükle
            Workbook workbook = new Workbook("example.xlsm", loadOptions);
            
            // Çalışma sayfasına eriş ve formül ayrıştırmanın atlandığını göster
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Console.WriteLine("Cell A1 formula: " + cell.Formula);
            Console.WriteLine("Cell A1 value: " + cell.Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


