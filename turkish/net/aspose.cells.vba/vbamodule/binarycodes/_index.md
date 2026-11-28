---
title: "VbaModule.BinaryCodes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaModule özelliği. Modülün ikili kodlarını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.vba/vbamodule/binarycodes/
---
## VbaModule.BinaryCodes property

Modülün ikili kodlarını alır ve ayarlar.

```csharp
public byte[] BinaryCodes { get; }
```

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyBinaryCodesDemo
    {
        public static void Run()
        {
            // VBA projesiyle birlikte çalışma kitabını yükleyin
            Workbook workbook = new Workbook("example.xlsm");
            
            // VBA projesine eriş
            VbaProject vbaProject = workbook.VbaProject;
            
            // İlk modülden ikili kodları alın
            byte[] binaryCodes = vbaProject.Modules[0].BinaryCodes;
            
            // Çince kodlama (936) kullanarak dizeye dönüştür
            string codeContent = Encoding.GetEncoding(936).GetString(binaryCodes);
            
            // Çince karakterler içeren içeriği çıktı olarak ver
            Console.WriteLine("VBA Module Content:");
            Console.WriteLine(codeContent);
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


