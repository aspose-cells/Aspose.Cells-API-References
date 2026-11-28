---
title: "WorkbookSettings.Region"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Çalışma kitabı için bölgesel ayarları alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/region/
---
## WorkbookSettings.Region property

Workbook için bölgesel ayarları alır veya ayarlar.

```csharp
public CountryCode Region { get; set; }
```

### Açıklamalar

1. Şablon dosyasından yüklenen bir çalışma kitabı için Aspose.Cells bileşeni tarafından kullanılan bölgesel ayarlar: i). XLS dosyası için, bölgesel ayarlar için tanımlı alanlar vardır ve MS Excel, XLS dosyasını kaydederken bölgesel ayar verilerini dosyaya kaydeder. Bu nedenle, çalışma kitabı için şablon dosyasındaki kaydedilmiş bölgeyi kullanırız. XLS dosyasında kaydedilmiş bölgeyi kullanmak istemiyorsanız, şablon dosyasını yükledikten sonra (örneğin CountryCode.Default gibi) beklenen bölgeye sıfırlayın. Ayrıca, bu yöntemle belirtilen kullanıcı değerini bir XLS dosyası kaydedilirken dosyaya da kaydederiz. ii). XLSX, XLSB... gibi diğer dosya formatları için, dosya formatı spesifikasyonunda bölgesel ayarlar için tanımlı bir alan yoktur. Bu yüzden, çalışma kitabı için uygulamanın ortamının bölgesel ayarlarını kullanırız. Ve, bu yöntemle belirtilen kullanıcı değeri, bu dosya formatlarıyla oluşturulan dosyalarda tutulamaz. 2. MS Excel'de görüntüleme etkisi için: Burada uygulanan bölgesel ayarlar yalnızca Aspose.Cells bileşeniyle çalışma zamanında etkili olur ve MS Excel ile oluşturulan dosya görüntülendiğinde etkili olmaz. Belirtilen bölgesel ayar verileri kaydedilmiş bir XLS dosyası için bile, MS Excel ile görüntülendiğinde/düzenlendiğinde, MS Excel'in biçimlendirme için kullandığı bölge her zaman MS Excel'in çalıştığı ortamın varsayılan bölgesel ayarlarıdır, dosyada kaydedilen bölge değil. Bu, MS Excel'in davranışıdır ve kodla değiştirilemez.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRegionDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Japan;
            
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(44089); // Represents 2020-09-15
            
            Style style = cell.GetStyle();
            style.Custom = "[$-F800]yyyy年m月d日";
            cell.SetStyle(style);
            
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


