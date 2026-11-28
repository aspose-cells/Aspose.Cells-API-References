---
title: "VbaProject.References"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProject özelliği. VBA projesinin tüm referanslarını alır"
type: docs
url: /tr/net/aspose.cells.vba/vbaproject/references/
---
## VbaProject.References property

VBA projesinin tüm referanslarını alır.

```csharp
public VbaProjectReferenceCollection References { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyReferencesDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluşturun (.xlsm dosyaları için VBA projesi otomatik olarak oluşturulur)
            Workbook workbook = new Workbook();
            
            // VBA proje referanslarına erişin (yalnızca çalışma kitabında VBA projesi varsa kullanılabilir)
            if (workbook.VbaProject != null)
            {
                VbaProjectReferenceCollection references = workbook.VbaProject.References;
                
                // Farklı türde referanslar ekleyin
                references.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
                references.AddControlRefrernce("MSForms", "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", "", "");
                references.AddProjectRefrernce("MyProject", "C:\\Projects\\MyProject.xlam", "..\\MyProject.xlam");

                // Referans sayısını göster
                Console.WriteLine($"Total references: {references.Count}");
            }

            // Makro etkin çalışma kitabı olarak kaydet
            workbook.Save("VbaProjectWithReferences.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProjectReferenceCollection](../../vbaprojectreferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


