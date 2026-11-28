---
title: "LoadOptions.DefaultStyleSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır"
type: docs
url: /tr/net/aspose.cells/loadoptions/defaultstylesettings/
---
## LoadOptions.DefaultStyleSettings property

Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Yükleme seçeneklerini varsayılan stil ayarlarıyla ayarla
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
            
            // Bir çalışma sayfası oluştur ve hücreleri al
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Varsayılan stili göstermek için değerleri ayarla
            cells["A1"].PutValue("Default Style Applied");
            cells["A2"].PutValue("Should have bottom alignment");
            
            // Özel stil ile bir hücre oluştur (varsayılanla karşılaştırmak için)
            Cell customCell = cells["B1"];
            customCell.PutValue("Custom Style");
            Style customStyle = customCell.GetStyle();
            customStyle.VerticalAlignment = TextAlignmentType.Center;
            customCell.SetStyle(customStyle);
            
            // Çalışma kitabını kaydedin
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
            
            // Stilleri doğrula
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("B1 Vertical Alignment: " + cells["B1"].GetStyle().VerticalAlignment);
        }
    }
}
```

### Ayrıca Bakınız

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


