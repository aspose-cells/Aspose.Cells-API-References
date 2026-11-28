---
title: "Enum VbaModuleType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Vba.VbaModuleType enum. VBA modülünün tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.vba/vbamoduletype/
---
## VbaModuleType enumeration

VBA modülünün tipini temsil eder.

```csharp
public enum VbaModuleType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Procedural | `0` | Procedural bir modülü temsil eder. |
| Document | `1` | Document bir modülü temsil eder. |
| Class | `2` | Class bir modülü temsil eder. |
| Designer | `3` | Designer bir modülü temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleTypeDemo
    {
        public static void VbaModuleTypeExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            
            // VBA projesini başlat
            VbaProject vbaProject = workbook.VbaProject;
            
            // Yeni bir sınıf modülü ekle
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "test");
            
            // VBA modülünü al
            VbaModule vbaModule = vbaProject.Modules[index];
            
            // Modül için kodları ayarla
            vbaModule.Codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub";
            
            // Excel dosyasını kaydet
            workbook.Save("VbaModuleTypeExample.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


