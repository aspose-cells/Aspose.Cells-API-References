---
title: "VbaModule.Codes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaModule özelliği. Modülün kodlarını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.vba/vbamodule/codes/
---
## VbaModule.Codes property

Modülün kodlarını alır ve ayarlar.

```csharp
public string Codes { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyCodesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir VBA modülü ekleyin
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            Aspose.Cells.Vba.VbaModule module = workbook.VbaProject.Modules[index];
            
            // İlk kodu ayarlayın
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello World\"\nEnd Sub";
            
            // Koda yeni satırlar ekleyerek değiştirin
            module.Codes = module.Codes + "\nSub AnotherMacro()\n    MsgBox \"Second Macro\"\nEnd Sub";
            
            // Çalışma kitabını kaydedin
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


