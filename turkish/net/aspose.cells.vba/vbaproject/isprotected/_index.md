---
title: "VbaProject.IsProtected"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProject özelliği. Bu VBA projesinin korunup korunmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.vba/vbaproject/isprotected/
---
## VbaProject.IsProtected property

Bu VBA projesinin korumalı olup olmadığını gösterir.

```csharp
public bool IsProtected { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Korumalı olmayan VBA projesi içeren örnek bir Excel dosyası yükleyin
            Workbook wb = new Workbook("load.xlsm");
            VbaProject vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // Korumalı VBA projesi içeren örnek bir Excel dosyası yükleyin
            wb = new Workbook("load_protected.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);

            // Korumalı ve kilitli VBA projesi içeren örnek bir Excel dosyası yükleyin
            wb = new Workbook("load_protected_lockedForView.xlsm");
            vbaProject = wb.VbaProject;
            Console.WriteLine("Is VBA Project Protected (load_protected_lockedForView.xlsm): " + vbaProject.IsProtected);
            Console.WriteLine("Is VBA Project Locked for Viewing: " + vbaProject.IslockedForViewing);
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


