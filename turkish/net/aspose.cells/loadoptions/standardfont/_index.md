---
title: "LoadOptions.StandardFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Varsayılan standart yazı tipi adını ayarlar"
type: docs
url: /tr/net/aspose.cells/loadoptions/standardfont/
---
## LoadOptions.StandardFont property

Varsayılan standart yazı tipi adını ayarlar

```csharp
[Obsolete("Use DefaultStyleSettings.FontName property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StandardFont { get; set; }
```

### Açıklamalar

NOTE: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen DefaultStyleSettings'i kullanın. Bu özellik, Mart 2022'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontDemo
    {
        public static void Run()
        {
            // Bellekte örnek bir Excel dosyası oluşturun
            MemoryStream ms = new MemoryStream();
            using (Workbook workbook = new Workbook())
            {
                workbook.Worksheets[0].Cells["A1"].PutValue("Standard Font Test");
                workbook.Save(ms, SaveFormat.Xlsx);
            }
            ms.Position = 0;

            // StandardFont ile yükleme seçeneklerini ayarlayın
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.StandardFont = "SimSun";
            
            // Belirtilen yazı tipiyle çalışma kitabını yükleyin
            Workbook workbookWithFont = new Workbook(ms, loadOptions);
            
            // Yazı tipinin ayarlandığını varsayılan stili kontrol ederek gösterin
            Console.WriteLine("Default font after loading: " + 
                workbookWithFont.DefaultStyle.Font.Name);
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


