---
title: "NumbersLoadOptions.NumbersLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NumbersLoadOptions yapıcı. Yapıcı"
type: docs
url: /tr/net/aspose.cells.numbers/numbersloadoptions/numbersloadoptions/
---
## NumbersLoadOptions constructor

Yapıcı.

```csharp
public NumbersLoadOptions()
```

### Örnekler

```csharp
using System;
using System.Globalization;
using Aspose.Cells;
using Aspose.Cells.Numbers;

namespace AsposeCellsExamples
{
    public class NumbersLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Yapıcıyı kullanarak NumbersLoadOptions oluştur
            NumbersLoadOptions loadOptions = new NumbersLoadOptions
            {
                // Bazı ortak özellikleri ayarla
                Password = "secure123",
                ParsingFormulaOnOpen = true,
                CultureInfo = new CultureInfo("en-US"),
                StandardFont = "Arial",
                MemorySetting = MemorySetting.MemoryPreference
            };

            // Çalışma kitabını seçeneklerle yükleyin
            Workbook workbook = new Workbook("sample.numbers", loadOptions);

            // XLSX olarak kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [NumbersLoadOptions](../)
* namespace [Aspose.Cells.Numbers](../../../aspose.cells.numbers/)
* assembly [Aspose.Cells](../../../)


