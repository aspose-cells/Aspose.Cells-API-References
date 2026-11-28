---
title: "HtmlLoadOptions.AttachedFilesDirectory"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlLoadOptions özelliği. Ekli dosyaların kaydedileceği dizin"
type: docs
url: /tr/net/aspose.cells/htmlloadoptions/attachedfilesdirectory/
---
## HtmlLoadOptions.AttachedFilesDirectory property

Ekli dosyaların kaydedileceği dizin.

```csharp
[Obsolete("Use HtmlLoadOptions.StreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AttachedFilesDirectory { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen HtmlLoadOptions.StreamProvider özelliğini kullanın. Bu özellik Aralık 2014'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // HtmlLoadOptions bir örnek oluştur.
            HtmlLoadOptions options = new HtmlLoadOptions();

            // Ekli dosyalar için dizini ayarlayın
            options.AttachedFilesDirectory = "C:\\AttachedFiles";

            // Belirtilen seçenekleri kullanarak bir HTML dosyasını Çalışma Kitabına yükleyin
            Workbook workbook = new Workbook("input.html", options);

            // Çalışma kitabını bir Excel dosyasına kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


