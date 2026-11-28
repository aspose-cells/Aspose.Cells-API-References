---
title: "VbaProjectReference.ExtendedLibid"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProjectReference özelliği. Referansın genişletilmiş Libid değerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.vba/vbaprojectreference/extendedlibid/
---
## VbaProjectReference.ExtendedLibid property

Referansın genişletilmiş Libid değerini alır ve ayarlar.

```csharp
public string ExtendedLibid { get; set; }
```

### Açıklamalar

Yalnızca kontrol referansı için.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferencePropertyExtendedLibidDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // VBA projesini başlat
                VbaProject vbaProject = workbook.VbaProject;

                // ExtendedLibid'i göstermek için bir kontrol referansı ekle
                vbaProject.References.AddControlRefrernce(
                    "SampleControl",
                    "{00020430-0000-0000-C000-000000000046}",
                    "stdole2.tlb",
                    "2.0");

                // İlk referansı al
                VbaProjectReference reference = vbaProject.References[0];

                // ExtendedLibid özelliği değerini göster
                Console.WriteLine("ExtendedLibid value: " + reference.ExtendedLibid);

                // ExtendedLibid'i ayarlamayı göster (çünkü okuma/yazma yapılabilir)
                reference.ExtendedLibid = "3.0";
                Console.WriteLine("Updated ExtendedLibid value: " + reference.ExtendedLibid);

                // Çalışma kitabını kaydedin
                workbook.Save("ExtendedLibidDemo.xlsm");
                Console.WriteLine("Workbook saved successfully with ExtendedLibid demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


