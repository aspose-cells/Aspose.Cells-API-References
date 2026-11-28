---
title: "HtmlTableLoadOption.TargetSheetIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlTableLoadOption özelliği. Tabloyun bulunacağı çalışma sayfasının hedef indeksini alın veya ayarlayın"
type: docs
url: /tr/net/aspose.cells/htmltableloadoption/targetsheetindex/
---
## HtmlTableLoadOption.TargetSheetIndex property

Tablonun yer alacağı çalışma sayfasının hedef indeksini alın veya ayarlayın.

```csharp
public int TargetSheetIndex { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTargetSheetIndexDemo
    {
        public static void Run()
        {
            // HTML yükleme seçenekleri oluştur
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            
            // TargetSheetIndex ile tablo yükleme seçeneklerini yapılandırın
            HtmlTableLoadOption tableLoadOption1 = new HtmlTableLoadOption();
            tableLoadOption1.Id = "table1";
            tableLoadOption1.TargetSheetIndex = 0; // Load to first worksheet
            
            HtmlTableLoadOption tableLoadOption2 = new HtmlTableLoadOption();
            tableLoadOption2.Id = "table2";
            tableLoadOption2.TargetSheetIndex = 1; // Load to second worksheet
            
            // Tablo yükleme seçenekleri ekle
            loadOptions.TableLoadOptions.Add(tableLoadOption1);
            loadOptions.TableLoadOptions.Add(tableLoadOption2);
            
            // Seçeneklerle HTML dosyasını yükleyin
            Workbook workbook = new Workbook("input.html", loadOptions);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Tabloların doğru sayfalara yüklendiğini doğrulayın
            Console.WriteLine("Table1 loaded to sheet index: " + tableLoadOption1.TargetSheetIndex);
            Console.WriteLine("Table2 loaded to sheet index: " + tableLoadOption2.TargetSheetIndex);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


