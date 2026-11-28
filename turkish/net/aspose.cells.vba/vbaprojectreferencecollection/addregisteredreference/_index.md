---
title: "VbaProjectReferenceCollection.AddRegisteredReference"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProjectReferenceCollection yöntemi. Bir Automation tip kitaplığına referans ekleyin"
type: docs
url: /tr/net/aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference/
---
## VbaProjectReferenceCollection.AddRegisteredReference method

Automation tip kitaplığına bir referans ekle.

```csharp
public int AddRegisteredReference(string name, string libid)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Referansın adı. |
| libid | String | Bir Automation tip kitaplığının tanımlayıcısı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddRegisteredReferenceWithStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // VBA projesine eriş
            VbaProject vbaProject = workbook.VbaProject;
            
            // stdole'a kayıtlı bir referans ekleyin
            vbaProject.References.AddRegisteredReference(
                "stdole", 
                "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


