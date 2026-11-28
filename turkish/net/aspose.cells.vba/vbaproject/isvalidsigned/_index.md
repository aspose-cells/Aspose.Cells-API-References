---
title: "VbaProject.IsValidSigned"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProject özelliği. VBA projesinin imzasının geçerli olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.vba/vbaproject/isvalidsigned/
---
## VbaProject.IsValidSigned property

VBA projesinin imzasının geçerli olup olmadığını gösterir.

```csharp
public bool IsValidSigned { get; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsValidSignedDemo
    {
        public static void Run()
        {
            // İmzalı VBA projesi içeren örnek bir çalışma kitabı yükleyin
            Workbook wb = new Workbook("example.xlsm");
            
            // VBA projesinin imzalı olup ve imzanın geçerli olduğunu kontrol edin
            Console.WriteLine("Is VBA Project Signed: " + wb.VbaProject.IsSigned);
            Console.WriteLine("Is Signature Valid: " + wb.VbaProject.IsValidSigned);

            // İmzayı kalıcı olduğunu doğrulamak için kaydedin ve yeniden yükleyin
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Excel97To2003);
            
            Workbook validateWb = new Workbook(ms);
            Console.WriteLine("After Reload - Is VBA Project Signed: " + validateWb.VbaProject.IsSigned);
            Console.WriteLine("After Reload - Is Signature Valid: " + validateWb.VbaProject.IsValidSigned);
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


