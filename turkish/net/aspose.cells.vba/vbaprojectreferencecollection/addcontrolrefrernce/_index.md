---
title: "VbaProjectReferenceCollection.AddControlRefrernce"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProjectReferenceCollection yöntemi. Çarpıtılmış bir tip kitaplığına ve onun genişletilmiş tip kitaplığına bir referans ekleyin"
type: docs
url: /tr/net/aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce/
---
## VbaProjectReferenceCollection.AddControlRefrernce method

Bükülmüş bir tip kitaplığına ve onun genişletilmiş tip kitaplığına bir referans ekle.

```csharp
[Obsolete("Use VbaProjectReferenceCollection.AddControlReferernce() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AddControlRefrernce(string name, string libid, string twiddledlibid, 
    string extendedLibid)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Referansın adı. |
| libid | String | Bir Automation tip kitaplığının tanımlayıcısı. |
| twiddledlibid | String | Çarpıtılmış bir tip kitaplığının tanımlayıcısı |
| extendedLibid | String | Genişletilmiş bir tip kitaplığının tanımlayıcısı |

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen VbaProjectReferenceCollection.AddControlReferernce() yöntemini kullanın. Bu yöntem Temmuz 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferenceCollectionMethodAddControlRefrernceWithStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;

            // Tüm string parametrelerle kontrol referansı ekleyin
            vbaProject.References.AddControlRefrernce(
                "MSForms",
                "*\\G{0D452EE1-E08F-101A-852E-02608C4D0BB4}#2.0#0#C:\\Windows\\system32\\FM20.DLL#Microsoft Forms 2.0 Object Library",
                "twiddledLibid",
                "extendedLibid");

            Console.WriteLine("Control reference added successfully. Total references: " + vbaProject.References.Count);
            
            workbook.Save("VbaProjectWithControlReference.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProjectReferenceCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


