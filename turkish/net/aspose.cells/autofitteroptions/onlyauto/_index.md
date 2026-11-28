---
title: "AutoFitterOptions.OnlyAuto"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFitterOptions özelliği. Yüksekliği özelleştirilmemiş satırların yalnızca otomatik olarak ayarlanıp ayarlanmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/autofitteroptions/onlyauto/
---
## AutoFitterOptions.OnlyAuto property

Yüksekliği özelleştirilmemiş satırların yalnızca ayarlanıp ayarlanmayacağını gösterir.

```csharp
public bool OnlyAuto { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyOnlyAutoDemo
    {
        public static void Run()
        {
            // Yükleme seçenekleri oluşturun ve OnlyAuto özelliğini ayarlayın
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = new AutoFitterOptions();
            loadOptions.AutoFitterOptions.OnlyAuto = true;

            // Çalışma kitabını otomatik ayarlama seçenekleriyle yükleyin
            Workbook workbook = new Workbook("example.xml", loadOptions);
            
            // Sütun genişliğini kontrol ederek otomatik ayarlamayı gösterin
            Console.WriteLine("Column width after auto-fit: " + 
                workbook.Worksheets[0].Cells.GetColumnWidthPixel(0));
            
            // Kalıcı olmayı doğrulamak için kaydet ve yeniden yükle
            workbook.Save("example_output.xlsx");
            Workbook reloaded = new Workbook("example_output.xlsx");
            Console.WriteLine("Reloaded column width: " + 
                reloaded.Worksheets[0].Cells.GetColumnWidthPixel(0));
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


