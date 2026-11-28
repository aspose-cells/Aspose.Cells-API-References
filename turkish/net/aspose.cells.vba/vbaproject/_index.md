---
title: "Sınıf VbaProject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Vba.VbaProject sınıfı. VBA projesini temsil eder"
type: docs
url: /tr/net/aspose.cells.vba/vbaproject/
---
## VbaProject class

VBA projesini temsil eder.

```csharp
public class VbaProject
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CertRawData](../../aspose.cells.vba/vbaproject/certrawdata/) { get; } | Bu VBA projesi imzalıysa sertifikanın ham verisini alır. |
| [Encoding](../../aspose.cells.vba/vbaproject/encoding/) { get; set; } | VBA projesinin kodlamasını alır ve ayarlar. |
| [IsLockedForView](../../aspose.cells.vba/vbaproject/islockedforview/) { get; } | Bu VBA projesinin görüntüleme için kilitli olup olmadığını gösterir. Doğruysa, kodlar görülemez. |
| [IslockedForViewing](../../aspose.cells.vba/vbaproject/islockedforviewing/) { get; } | (**Obsolete.**) Bu VBA projesinin görüntüleme için kilitli olup olmadığını gösterir. |
| [IsProtected](../../aspose.cells.vba/vbaproject/isprotected/) { get; } | Bu VBA projesinin korumalı olup olmadığını gösterir. |
| [IsSigned](../../aspose.cells.vba/vbaproject/issigned/) { get; } | VBAcode'un imzalı olup olmadığını gösterir. |
| [IsValidSigned](../../aspose.cells.vba/vbaproject/isvalidsigned/) { get; } | VBA projesinin imzasının geçerli olup olmadığını gösterir. |
| [Modules](../../aspose.cells.vba/vbaproject/modules/) { get; } | Tüm [`VbaModule`](../vbamodule/) nesnelerini alır. |
| [Name](../../aspose.cells.vba/vbaproject/name/) { get; set; } | VBA projesinin adını alır ve ayarlar. |
| [References](../../aspose.cells.vba/vbaproject/references/) { get; } | VBA projesinin tüm referanslarını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Copy](../../aspose.cells.vba/vbaproject/copy/)(VbaProject) | VBA projesini başka bir dosyadan kopyalar. |
| [Protect](../../aspose.cells.vba/vbaproject/protect/)(bool, string) | Bu VBA projesini korur veya korumasını kaldırır. |
| [Sign](../../aspose.cells.vba/vbaproject/sign/)(DigitalSignature) | Bu VBA projesini bir DigitalSignature ile imzalar |
| [ValidatePassword](../../aspose.cells.vba/vbaproject/validatepassword/)(string) | Koruma şifresini doğrular. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Text;
    using System.Security.Cryptography.X509Certificates;

    public class VbaProjectDemo
    {
        public static void VbaProjectExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // VBA projesini başlat
            VbaProject vbaProject = workbook.VbaProject;

            // Özellikleri ayarlama
            vbaProject.Name = "MyVbaProject";
            vbaProject.Encoding = Encoding.UTF8;

            // Salt okunur özellikler kontrol ediliyor.
            bool isSigned = vbaProject.IsSigned;
            bool isProtected = vbaProject.IsProtected;
            bool isLockedForViewing = vbaProject.IslockedForViewing;
            bool isValidSigned = vbaProject.IsValidSigned;

            // Bir VBA modülü ekleniyor.
            int moduleIndex = vbaProject.Modules.Add(VbaModuleType.Class, "MyModule");

            // Bir VBA proje referansı ekleniyor.
            vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");

            // VBA projesi korunuyor.
            vbaProject.Protect(true, "password");

            // VBA projesi imzalanıyor.
            X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "certificate_password");
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Signature Comments", DateTime.Now);
            vbaProject.Sign(digitalSignature);

            // Excel dosyasını kaydetme
            workbook.Save("VbaProjectExample.xlsm");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


