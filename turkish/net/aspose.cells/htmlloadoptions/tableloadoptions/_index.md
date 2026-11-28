---
title: "HtmlLoadOptions.TableLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlLoadOptions özelliği. HtmlTableLoadOptionCollection örneğini alın"
type: docs
url: /tr/net/aspose.cells/htmlloadoptions/tableloadoptions/
---
## HtmlLoadOptions.TableLoadOptions property

HtmlTableLoadOptionCollection örneğini al

```csharp
public HtmlTableLoadOptionCollection TableLoadOptions { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyTableLoadOptionsDemo
    {
        public static void Run()
        {
            // HTML yükleme seçenekleri oluştur
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.SupportDivTag = true;
            
            // Tablo yükleme seçeneklerini indeksle ekleyin
            loadOptions.TableLoadOptions.Add(1);
            loadOptions.TableLoadOptions.Add(2);
            
            // ID'ye göre tablo yükleme seçeneklerini ekle
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table1";
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "table2";
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // Seçeneklerle HTML dosyasını yükleyin
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Çıktıyı kaydet
            workbook.Save("output.xlsx");
            
            // Temizle ve yeni tablo yükleme seçeneklerini ekle
            loadOptions.TableLoadOptions.Clear();
            
            // Sayfa indeks eşlemesiyle tablo yükleme seçeneklerini ekle
            loadOptions.TableLoadOptions.Add(0, 2); // Table index 0 -> Sheet 2
            loadOptions.TableLoadOptions.Add(1, 0); // Table index 1 -> Sheet 0
            
            // ID ve sayfa eşlemesiyle tablo yükleme seçeneklerini ekle
            tableLoadOption = new HtmlTableLoadOption();
            tableLoadOption.Id = "mainTable";
            tableLoadOption.TargetSheetIndex = 1;
            loadOptions.TableLoadOptions.Add(tableLoadOption);
            
            // Yeni seçeneklerle tekrar yükle ve kaydet
            workbook = new Workbook("input.html", loadOptions);
            workbook.Save("output_mapped.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOptionCollection](../../htmltableloadoptioncollection/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


