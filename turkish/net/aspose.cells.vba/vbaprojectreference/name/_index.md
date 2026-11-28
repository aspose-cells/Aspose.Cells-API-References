---
title: "VbaProjectReference.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProjectReference özelliği. Referansın adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.vba/vbaprojectreference/name/
---
## VbaProjectReference.Name property

Referansın adını alır ve ayarlar.

```csharp
public string Name { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaProjectReferencePropertyNameDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur (VBA projesi .xlsm dosyaları için otomatik olarak oluşturulur)
            Workbook workbook = new Workbook(FileFormatType.Xlsm);
            
            // VBA projesine bir referans ekle
            string referenceName = "MyReference";
            string referencePath = @"C:\Temp\MyLibrary.dll";
            workbook.VbaProject.References.AddRegisteredReference(referenceName, referencePath);

            // Referansı Name özelliğiyle eriş ve doğrula
            VbaProjectReferenceCollection references = workbook.VbaProject.References;
            for (int i = 0; i < references.Count; i++)
            {
                if (references[i].Name.Equals(referenceName))
                {
                    Console.WriteLine($"Found reference: {references[i].Name}");
                    break;
                }
            }

            // Çalışma kitabını kaydedin
            workbook.Save("VbaProjectReferenceDemo.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


