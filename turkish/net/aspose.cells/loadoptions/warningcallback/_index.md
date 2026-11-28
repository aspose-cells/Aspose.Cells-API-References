---
title: "LoadOptions.WarningCallback"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Uyarı geri çağrısını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/loadoptions/warningcallback/
---
## LoadOptions.WarningCallback property

Uyarı geri çağrısını alır veya ayarlar.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomWarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine($"Warning: {warningInfo.Description}");
        }
    }

    public class LoadOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Özel bir uyarı geri çağrısı oluşturun
            IWarningCallback warningCallback = new CustomWarningCallback();

            // Uyarı geri çağrısı ile yükleme seçeneklerini başlatın
            LoadOptions options = new LoadOptions();
            options.WarningCallback = warningCallback;
            options.IgnoreUselessShapes = true;

            // Seçeneklerle çalışma kitabını yükle
            Workbook workbook = new Workbook("example.xlsx", options);

            // Bir hücreye erişerek uyarı geri çağrısı kullanımını gösterin
            Console.WriteLine($"Cell value: {workbook.Worksheets[0].Cells["A1"].StringValue}");

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* interface [IWarningCallback](../../iwarningcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


