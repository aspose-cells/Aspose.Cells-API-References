---
title: "VbaModule.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaModule özelliği. Modülün tipini alır"
type: docs
url: /tr/net/aspose.cells.vba/vbamodule/type/
---
## VbaModule.Type property

Modülün tipini alır.

```csharp
public VbaModuleType Type { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyTypeDemo
    {
        public static void Run()
        {
            // Makro etkin örnek dosyayla bir çalışma kitabı oluşturun
            Workbook wb = new Workbook("example.xlsm");
            
            // VBA projesine ve modüllere erişin
            VbaProject vbaProject = wb.VbaProject;
            VbaModuleCollection modules = vbaProject.Modules;
            
            // Modül tiplerini ve adlarını gösterin
            for (int i = 0; i < modules.Count; i++)
            {
                Console.WriteLine($"Module Name: {modules[i].Name}");
                Console.WriteLine($"Module Type: {modules[i].Type}");
                Console.WriteLine();
            }
            
            wb.Save("output.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


