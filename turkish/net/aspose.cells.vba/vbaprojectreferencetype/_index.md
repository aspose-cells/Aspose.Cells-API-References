---
title: "Enum VbaProjectReferenceType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Vba.VbaProjectReferenceType enum. VBA proje referansının tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.vba/vbaprojectreferencetype/
---
## VbaProjectReferenceType enumeration

VBA proje referansının tipini temsil eder.

```csharp
public enum VbaProjectReferenceType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Registered | `0` | Bir Automation tip kitaplığına referans belirtir. |
| Control | `1` | Twiddled tip kitaplığına ve onun genişletilmiş tip kitaplığına referans belirtir. |
| Project | `2` | Harici bir VBA projesine referans belirtir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferenceTypeDemo
    {
        public static void VbaProjectReferenceTypeExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // VBA projesini başlat
            VbaProject vbaProject = workbook.VbaProject;

            // VBA proje referansı ekle
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // Excel dosyasını kaydetme
            workbook.Save("VbaProjectReferenceTypeExample.xlsm");

            // VbaProjectReferenceType enum kullanımını gösterme
            VbaProjectReference reference = vbaProject.References[0];
            Console.WriteLine("Reference Type: " + reference.Type);
            Console.WriteLine("Reference Name: " + reference.Name);
            Console.WriteLine("Reference Libid: " + reference.Libid);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


