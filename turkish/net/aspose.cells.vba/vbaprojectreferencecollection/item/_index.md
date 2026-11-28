---
title: "VbaProjectReferenceCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProjectReferenceCollection özelliği. Listedeki referansı indeks ile alın"
type: docs
url: /tr/net/aspose.cells.vba/vbaprojectreferencecollection/item/
---
## VbaProjectReferenceCollection indexer

Listedeki referansı indeksine göre al.

```csharp
public VbaProjectReference this[int i] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| i | İndeks. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // VBA projesini başlat
            VbaProject vbaProject = workbook.VbaProject;
            
            // VBA projesine referanslar ekleyin
            vbaProject.References.AddRegisteredReference("stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            vbaProject.References.AddControlRefrernce("MSForms", 
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library", 
                "twiddledLibid", "extendedLibid");
            
            // Referans koleksiyonunu alın
            VbaProjectReferenceCollection references = vbaProject.References;
            
            // Item özelliğini kullanarak referanslara erişin
            VbaProjectReference firstRef = references[0];
            VbaProjectReference secondRef = references[1];
            
            Console.WriteLine("First Reference: " + firstRef.Name);
            Console.WriteLine("Second Reference: " + secondRef.Name);
            
            // Çalışma kitabını kaydedin
            workbook.Save("VbaProjectReferences.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProjectReference](../../vbaprojectreference/)
* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


