---
title: "NumbersLoadOptions.LoadTableType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NumbersLoadOptions özelliği. Tek bir çalışma sayfasında birden fazla tablo yükleme türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.numbers/numbersloadoptions/loadtabletype/
---
## NumbersLoadOptions.LoadTableType property

Bir çalışma sayfasında birden fazla tabloyu yükleme türünü alır ve ayarlar.

```csharp
public LoadNumbersTableType LoadTableType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsPropertyLoadTableTypeDemo
    {
        public static void Run()
        {
            // NumbersLoadOptions örneği oluştur
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // LoadTableType özelliğinin kullanımını göster
                LoadTableType = LoadNumbersTableType.OneTablePerSheet,
                
                // Diğer minimum gerekli özellikler
                Password = "password123",
                ParsingFormulaOnOpen = true
            };

            // Belirtilen yükleme seçenekleriyle bir Numbers dosyası yükle
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // Çalışma kitabını XLSX formatında kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [LoadNumbersTableType](../../loadnumberstabletype/)
* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


