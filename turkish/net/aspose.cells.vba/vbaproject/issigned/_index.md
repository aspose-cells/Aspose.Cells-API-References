---
title: "VbaProject.IsSigned"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProject özelliği. VBA kodunun imzalı olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.vba/vbaproject/issigned/
---
## VbaProject.IsSigned property

VBAcode'un imzalı olup olmadığını gösterir.

```csharp
public bool IsSigned { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsSignedDemo
    {
        public static void Run()
        {
            // VBA projesi içeren örnek bir Excel dosyası yükleyin
            Workbook workbook = new Workbook("example.xlsm");
            
            // VBA projesinin imzalı olup olmadığını kontrol edin
            if (workbook.VbaProject.IsSigned)
            {
                Console.WriteLine("VBA project is signed.");
                Console.WriteLine("Signature is valid: " + workbook.VbaProject.IsValidSigned);
            }
            else
            {
                Console.WriteLine("VBA project is not signed.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


