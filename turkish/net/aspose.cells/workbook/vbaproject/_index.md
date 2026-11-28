---
title: "Workbook.VbaProject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Bir elektronik tabloda VbaProject'i alır"
type: docs
url: /tr/net/aspose.cells/workbook/vbaproject/
---
## Workbook.VbaProject property

Bir elektronik tabloda `VbaProject`'i alır.

```csharp
public VbaProject VbaProject { get; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyVbaProjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // VBA projesine erişin (VbaProject yalnızca okunabilir, yalnızca var olup olmadığını kontrol edebiliriz)
            if (workbook.VbaProject == null)
            {
                // Makro etkin çalışma kitabı olarak kaydederek VBA projesi oluşturun
                workbook.Save("temp.xlsm", SaveFormat.Xlsm);
                workbook = new Workbook("temp.xlsm");
                File.Delete("temp.xlsm");
            }

            // VBA projesine yeni bir modül ekleyin
            int moduleIndex = workbook.VbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Eklenen modülü alın ve kodunu ayarlayın
            VbaModule module = workbook.VbaProject.Modules[moduleIndex];
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";

            // Çalışma kitabını kaydedin
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "VbaProjectDemo.xlsm");
            workbook.Save(outputPath, SaveFormat.Xlsm);
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProject](../../../aspose.cells.vba/vbaproject/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


