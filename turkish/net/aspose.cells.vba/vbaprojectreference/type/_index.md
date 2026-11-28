---
title: "VbaProjectReference.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProjectReference özelliği. Bu referansın tipini alır"
type: docs
url: /tr/net/aspose.cells.vba/vbaprojectreference/type/
---
## VbaProjectReference.Type property

Bu referansın tipini alır.

```csharp
public VbaProjectReferenceType Type { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // VBA projesini başlat
            VbaProject vbaProject = workbook.VbaProject;

            // VBA projesine kayıtlı bir referans ekle
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // İlk referansı al ve Type özelliğini göster
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);

            // Çalışma kitabını kaydedin
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* enum [VbaProjectReferenceType](../../vbaprojectreferencetype/)
* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


