---
title: "VbaProjectReferenceCollection.AddProjectRefrernce"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProjectReferenceCollection yöntemi. Harici bir VBA projesine referans ekler"
type: docs
url: /tr/net/aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce/
---
## VbaProjectReferenceCollection.AddProjectRefrernce method

Harici bir VBA projesine bir referans ekler.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddProjectReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddProjectRefrernce(string name, string absoluteLibid, string relativeLibid)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Referansın adı. |
| absoluteLibid | String | Mutlak bir yol ile referans verilen VBA projesinin tanımlayıcısı. |
| relativeLibid | String | Göreceli bir yol ile referans verilen VBA projesinin tanımlayıcısı |

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen VbaProjectReferenceCollection.AddProjectReferernce() yöntemini kullanın. Bu yöntem Temmuz 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddProjectRefrernceWithStringStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // VBA projesini başlat
            VbaProject vbaProject = workbook.VbaProject;
            
            // Mutlak ve göreceli libid'lerle bir proje referansı ekleyin
            vbaProject.References.AddProjectRefrernce("MyProject", "absoluteLibid", "relativeLibid");
            
            // Referans sayısını göster
            Console.WriteLine("Total References: " + vbaProject.References.Count);
            
            // Çalışma kitabını kaydedin
            workbook.Save("VbaProjectReferenceExample.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


