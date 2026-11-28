---
title: "Sınıf IndividualFontConfigs"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.IndividualFontConfigs sınıfı. Her Workbook nesnesi için font yapılandırmaları"
type: docs
url: /tr/net/aspose.cells/individualfontconfigs/
---
## IndividualFontConfigs class

Her [`Workbook`](../workbook/) nesnesi için font yapılandırmaları.

```csharp
public class IndividualFontConfigs
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [IndividualFontConfigs](individualfontconfigs/)() | Yapıcı. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetFontSources](../../aspose.cells/individualfontconfigs/getfontsources/)() | Kaynakların listesini içeren dizinin bir kopyasını alır |
| [GetFontSubstitutes](../../aspose.cells/individualfontconfigs/getfontsubstitutes/)(string) | Orijinal font mevcut değilse kullanılacak font ikame adlarını içeren bir dizi döndürür. |
| [SetFontFolder](../../aspose.cells/individualfontconfigs/setfontfolder/)(string, bool) | Yazı tipleri klasörünü ayarlar |
| [SetFontFolders](../../aspose.cells/individualfontconfigs/setfontfolders/)(string[], bool) | Font klasörlerini ayarlar |
| [SetFontSources](../../aspose.cells/individualfontconfigs/setfontsources/)(FontSourceBase[]) | Yazı tipi kaynaklarını ayarlar. |
| [SetFontSubstitutes](../../aspose.cells/individualfontconfigs/setfontsubstitutes/)(string, string[]) | Belirli bir orijinal font adı için font ikame adlarını ayarlar. |

### Örnekler

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassIndividualFontConfigsDemo
    {
        public static void Run()
        {
            // Font kaynakları için geçici dizinler oluştur
            string tempFontFolder1 = Path.Combine(Path.GetTempPath(), "FontFolder1_" + Guid.NewGuid().ToString());
            string tempFontFolder2 = Path.Combine(Path.GetTempPath(), "FontFolder2_" + Guid.NewGuid().ToString());
            Directory.CreateDirectory(tempFontFolder1);
            Directory.CreateDirectory(tempFontFolder2);

            // Örnek CSV dosyası oluştur
            string csvFilePath = "sample_data.csv";
            File.WriteAllText(csvFilePath, "Name,Age\nJohn,30\nAlice,25", Encoding.UTF8);

            try
            {
                // Font yapılandırmasını başlat
                IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

                // Arial için font ikamelerini ayarla
                fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Verdana" });

                // Font dizinlerini yapılandır
                fontConfigs.SetFontFolder(tempFontFolder1, false);
                fontConfigs.SetFontFolders(new string[] { tempFontFolder1, tempFontFolder2 }, true);

                // Font kaynaklarını yapılandır
                FontSourceBase[] fontSources = {
                    new FolderFontSource(tempFontFolder1, false),
                    new FolderFontSource(tempFontFolder2, true)
                };
                fontConfigs.SetFontSources(fontSources);

                // Yazı tipı yapılandırmalarıyla metin yükleme seçenekleri oluşturun
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
                {
                    FontConfigs = fontConfigs
                };

                // Yapılandırılmış seçeneklerle çalışma kitabını yükle
                using (Workbook workbook = new Workbook(csvFilePath, loadOptions))
                {
                    // Excel dosyası olarak kaydet
                    workbook.Save("output_with_font_config.xlsx");
                }
            }
            finally
            {
                // Geçici kaynakları temizle
                if (Directory.Exists(tempFontFolder1)) Directory.Delete(tempFontFolder1, true);
                if (Directory.Exists(tempFontFolder2)) Directory.Delete(tempFontFolder2, true);
                if (File.Exists(csvFilePath)) File.Delete(csvFilePath);
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


