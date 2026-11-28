---
title: "VbaProject.Modules"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProject özelliği. Tüm VbaModule nesnelerini alır"
type: docs
url: /tr/net/aspose.cells.vba/vbaproject/modules/
---
## VbaProject.Modules property

Tüm [`VbaModule`](../../vbamodule/) nesnelerini alır.

```csharp
public VbaModuleCollection Modules { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyModulesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;
            
            // Yeni bir modül ekleyin ve Modules özelliğini kullanarak alın
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            
            // Modüle kod ekleyin
            module.Codes = "Sub Test()\r\n    MsgBox \"Module demonstration\"\r\nEnd Sub";
            
            // Makro etkin formatta kaydedin
            workbook.Save("VbaModulesDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


