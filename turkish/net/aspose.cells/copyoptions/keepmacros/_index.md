---
title: "CopyOptions.KeepMacros"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CopyOptions özelliği. Makroların tutulup tutulmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/copyoptions/keepmacros/
---
## CopyOptions.KeepMacros property

Makroların korunup korunmayacağını gösterir;

```csharp
public bool KeepMacros { get; set; }
```

### Açıklamalar

Yalnızca çalışma kitabı kopyalamak için.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyKeepMacrosDemo
    {
        public static void Run()
        {
            // Makrolu kaynak çalışma kitabı oluşturun (makrolar içeren bir şablon dosyası kullanarak)
            Workbook srcWorkbook = new Workbook("macros_template.xlsm");
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Macro-enabled source");

            // Hedef çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook();
            
            // KeepMacros true ile kopya seçeneklerini ayarlayın
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;

            // Makrolu çalışma sayfasını kopyalayın
            destWorkbook.Worksheets[0].Copy(srcSheet, options);

            // Sonucu kaydedin
            destWorkbook.Save("KeepMacrosExample.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


