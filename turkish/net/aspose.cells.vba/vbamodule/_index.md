---
title: "Sınıf VbaModule"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Vba.VbaModule sınıfı. VBA projesindeki modülü temsil eder"
type: docs
url: /tr/net/aspose.cells.vba/vbamodule/
---
## VbaModule class

VBA projesindeki modülü temsil eder.

```csharp
public class VbaModule
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BinaryCodes](../../aspose.cells.vba/vbamodule/binarycodes/) { get; } | Modülün ikili kodlarını alır ve ayarlar. |
| [Codes](../../aspose.cells.vba/vbamodule/codes/) { get; set; } | Modülün kodlarını alır ve ayarlar. |
| [Name](../../aspose.cells.vba/vbamodule/name/) { get; set; } | Modülün adını alır ve ayarlar. |
| [Type](../../aspose.cells.vba/vbamodule/type/) { get; } | Modülün tipini alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleDemo
    {
        public static void VbaModuleExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // VBA projesini başlat
            VbaProject vbaProject = workbook.VbaProject;

            // Yeni bir modül ekle
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");

            // VBA modülünü al
            VbaModule vbaModule = vbaProject.Modules[index];

            // Modül için kodları ayarla
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";

            // Excel dosyasını kaydetme
            workbook.Save("VbaModuleExample.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


