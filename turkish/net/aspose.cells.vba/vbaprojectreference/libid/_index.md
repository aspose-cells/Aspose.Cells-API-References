---
title: "VbaProjectReference.Libid"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProjectReference özelliği. Referansın Libid değerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.vba/vbaprojectreference/libid/
---
## VbaProjectReference.Libid property

Referansın Libid değerini alır ve ayarlar.

```csharp
public string Libid { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyLibidDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook targetWorkbook = new Workbook();
            
            // VBA projesi içeren kaynak çalışma kitabını yükleyin
            Workbook sourceWorkbook = new Workbook("source.xlsm");
            
            // Hedefteki mevcut referansları temizleyin
            targetWorkbook.VbaProject.References.Clear();
            
            // Kaynak'tan hedefe referansları kopyala
            foreach (VbaProjectReference reference in sourceWorkbook.VbaProject.References)
            {
                if (reference.Type == VbaProjectReferenceType.Registered)
                {
                    // Libid özelliği kullanımını göster
                    targetWorkbook.VbaProject.References.AddRegisteredReference(reference.Name, reference.Libid);
                }
                else if (reference.Type == VbaProjectReferenceType.Control)
                {
                    targetWorkbook.VbaProject.References.AddControlRefrernce(
                        reference.Name, 
                        reference.Libid, 
                        reference.Twiddledlibid, 
                        reference.ExtendedLibid);
                }
            }
            
            // Sonucu kaydet
            targetWorkbook.Save("output.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


