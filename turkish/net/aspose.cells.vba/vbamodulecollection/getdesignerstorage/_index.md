---
title: "VbaModuleCollection.GetDesignerStorage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaModuleCollection yöntemi. Tasarımcının verilerini temsil eder"
type: docs
url: /tr/net/aspose.cells.vba/vbamodulecollection/getdesignerstorage/
---
## VbaModuleCollection.GetDesignerStorage method

Tasarımcının verilerini temsil eder.

```csharp
public byte[] GetDesignerStorage(string name)
```

### Açıklamalar

Bunları ayrıştırmayı desteklemiyoruz. Yalnızca kopyalamak için.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodGetDesignerStorageWithStringDemo
    {
        public static void Run()
        {
            // VBA projesiyle bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            
            // Bir tasarımcı modülü ekleyin
            int index = workbook.VbaProject.Modules.Add(VbaModuleType.Designer, "TestForm");
            
            // Tasarımcı depolamasını alın (başlangıçta null olacaktır)
            byte[] storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Initial designer storage: " + (storage == null ? "null" : "exists"));
            
            // Bazı tasarımcı depolama verileri ekleyin
            byte[] sampleData = new byte[] { 0x01, 0x02, 0x03 };
            workbook.VbaProject.Modules.AddDesignerStorage("TestForm", sampleData);
            
            // Tasarımcı depolamasını alın ve görüntüleyin
            storage = workbook.VbaProject.Modules.GetDesignerStorage("TestForm");
            Console.WriteLine("Storage after adding: " + (storage == null ? "null" : BitConverter.ToString(storage)));
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


