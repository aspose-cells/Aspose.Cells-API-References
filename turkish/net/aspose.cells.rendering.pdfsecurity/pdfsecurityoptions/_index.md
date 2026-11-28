---
title: "Sınıf PdfSecurityOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.PdfSecurity.PdfSecurityOptions class. Bir PDF belgesi için şifreleme ve erişim izinleri seçenekleri. PDF/A güvenlik ayarına izin vermez."
type: docs
url: /tr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/
---
## PdfSecurityOptions class

Bir PDF belgesi için şifreleme ve erişim izinleri seçenekleri. PDF/A güvenlik ayarına izin vermez.

```csharp
public class PdfSecurityOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [PdfSecurityOptions](pdfsecurityoptions/)() | PdfSecurityOptions yapıcısı |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AccessibilityExtractContent](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/) { get; set; } | Metin ve grafik çıkarılmasına izin verilip verilmediğini gösterir (engelli kullanıcılar için erişilebilirliği destekleme veya diğer amaçlar için). |
| [AnnotationsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/) { get; set; } | Metin açıklamaları eklenmesine veya değiştirilmesine, etkileşimli form alanlarının doldurulmasına izin verilip verilmediğini gösterir. |
| [AssembleDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/) { get; set; } | Belgenin birleştirilmesine (sayfaları ekleme, döndürme veya silme ve yer imleri ya da küçük resimler oluşturma) izin verilip verilmediğini gösterir, hatta [`ModifyDocumentPermission`](./modifydocumentpermission/) açık olsa bile. |
| [ExtractContentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/) { get; set; } | Belgeden metin ve grafikleri, [`AccessibilityExtractContent`](./accessibilityextractcontent/) tarafından kontrol edilen işlemler dışındaki işlemlerle kopyalama veya çıkarma izni verilip verilmediğini gösterir. |
| [ExtractContentPermissionObsolete](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/) { get; set; } | (**Obsolete.**) İçeriği kopyalama veya çıkarma izni PDF referansına göre kullanımdan kaldırıldı. |
| [FillFormsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/) { get; set; } | Mevcut etkileşimli form alanlarını (imza alanları dahil) doldurmaya izin verilip verilmediğini gösterir, hatta [`ModifyDocumentPermission`](./modifydocumentpermission/) açık olsa bile. |
| [FullQualityPrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/) { get; set; } | PDF içeriğinin doğru bir dijital kopyası oluşturulabilecek bir temsile belgeyi yazdırmaya izin verilip verilmediğini gösterir. |
| [ModifyDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/) { get; set; } | Belgenin içeriğini, [`AnnotationsPermission`](./annotationspermission/), [`FillFormsPermission`](./fillformspermission/) ve [`AssembleDocumentPermission`](./assembledocumentpermission/) tarafından kontrol edilen işlemler dışındaki işlemlerle değiştirmeye izin verilip verilmediğini gösterir. |
| [OwnerPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/) { get; set; } | Şifrelenmiş PDF belgesi için sahibi şifresini alır veya ayarlar. |
| [PrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/) { get; set; } | Belgeyi yazdırmaya izin verilip verilmediğini gösterir. |
| [UserPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/) { get; set; } | Şifrelenmiş PDF belgesini açmak için gereken kullanıcı şifresini alır veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Rendering.PdfSecurity;
    using System;

    public class PdfSecurityOptionsDemo
    {
        public static void PdfSecurityOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Aspose";

            // PdfSaveOptions oluştur
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // PdfSecurityOptions oluştur
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            // Güvenlik seçeneklerini ayarlayın
            pdfSecurityOptions.OwnerPassword = "YourOwnerPassword";
            pdfSecurityOptions.UserPassword = "YourUserPassword";
            pdfSecurityOptions.PrintPermission = true;
            pdfSecurityOptions.ModifyDocumentPermission = false;
            pdfSecurityOptions.ExtractContentPermissionObsolete = false;
            pdfSecurityOptions.AnnotationsPermission = true;
            pdfSecurityOptions.FillFormsPermission = true;
            pdfSecurityOptions.ExtractContentPermission = false;
            pdfSecurityOptions.AccessibilityExtractContent = true;
            pdfSecurityOptions.AssembleDocumentPermission = false;
            pdfSecurityOptions.FullQualityPrintPermission = true;

            // PdfSaveOptions'a güvenlik seçeneklerini ata
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Çalışma kitabını belirtilen güvenlik seçenekleriyle PDF olarak kaydet
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering.PdfSecurity](../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../)


