---
title: "VbaProject.Encoding"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaProject özelliği. VBA projesinin kodlamasını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.vba/vbaproject/encoding/
---
## VbaProject.Encoding property

VBA projesinin kodlamasını alır ve ayarlar.

```csharp
public Encoding Encoding { get; set; }
```

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Vba;
using System.Security.Cryptography.X509Certificates;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyEncodingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // VBA projesini başlat
            VbaProject vbaProject = workbook.VbaProject;

            // Kodlama dahil olmak üzere VBA proje özelliklerini ayarlayın
            vbaProject.Name = "TestVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // VBA projesine bir modül ekleyin
            vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");

            // VBA projesiyle birlikte çalışma kitabını kaydedin
            workbook.Save("VbaProjectEncodingDemo.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


