---
title: "HtmlSaveOptions.ExcludeUnusedStyles"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Kullanılmayan stillerin dışarıda bırakılıp bırakılmayacağını gösterir. Oluşturulan HTML dosyalarında kullanılmayan stillerin dışarıda bırakılması, görsel etkilere zarar vermeden dosya boyutunu küçültebilir. Bu nedenle bu özelliğin varsayılan değeri true'tir. Kullanıcı, oluşturulan HTML için çalışma kitabındaki tüm stilleri koruması gerektiğinde, örneğin daha sonra oluşturulan HTML'den çalışma kitabını geri yüklemesi gerektiği senaryoda, lütfen bu özelliği false olarak ayarlayın."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/excludeunusedstyles/
---
## HtmlSaveOptions.ExcludeUnusedStyles property

Kullanılmayan stillerin dışarıda bırakılıp bırakılmadığını gösterir. Oluşturulan HTML dosyalarında kullanılmayan stillerin dışarıda bırakılması, görsel etkilere zarar vermeden dosya boyutunu küçültebilir. Bu nedenle bu özelliğin varsayılan değeri true'tır. Kullanıcı, oluşturulan HTML'den (örneğin, daha sonra HTML'den çalışma kitabını geri yüklemek gerektiğinde) çalışma kitabındaki tüm stilleri korumak istiyorsa, lütfen bu özelliği false olarak ayarlayın.

```csharp
public bool ExcludeUnusedStyles { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExcludeUnusedStylesDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Farklı stillerle örnek veri ekleyin
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.Value = "Styled text";
            Style style1 = cell1.GetStyle();
            style1.Font.Color = Color.Red;
            style1.Font.IsBold = true;
            cell1.SetStyle(style1);

            Cell cell2 = workbook.Worksheets[0].Cells["A2"];
            cell2.Value = "Different style";
            Style style2 = cell2.GetStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            cell2.SetStyle(style2);

            // Kullanılmayan stilleri dışarıda bırakmak için HTML kaydetme seçeneklerini yapılandırın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExcludeUnusedStyles = true;

            // Çalışma kitabını HTML seçenekleriyle kaydet
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with ExcludeUnusedStyles=true");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


