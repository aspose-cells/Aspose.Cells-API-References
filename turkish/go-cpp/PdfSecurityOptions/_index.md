---
title: "PdfSecurityOptions Sınıfı"
linktitle: "PdfSecurityOptions"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "PdfSecurityOptions sınıfı. Go'da pdfsecurityoptions'i temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/pdfsecurityoptions/
---

## PdfSecurityOptions class

Bir PDF belgesi için şifreleme ve erişim izinleri seçenekleri.PDF/A güvenlik ayarına izin vermez.

```go

type PdfSecurityOptions struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewPdfSecurityOptions](./newpdfsecurityoptions/) | PdfSecurityOptions yapıcı metodu |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetUserPassword](./getuserpassword/) | Şifreli PDF belgesini açmak için gereken kullanıcı şifresini alır veya ayarlar. |
| [SetUserPassword](./setuserpassword/) | Şifreli PDF belgesini açmak için gereken kullanıcı şifresini alır veya ayarlar. |
| [GetOwnerPassword](./getownerpassword/) | Şifreli PDF belgesi için sahibi şifresini alır veya ayarlar. |
| [SetOwnerPassword](./setownerpassword/) | Şifreli PDF belgesi için sahibi şifresini alır veya ayarlar. |
| [GetPrintPermission](./getprintpermission/) | Belgenin yazdırılmasına izin verilip verilmeyeceğini gösterir. |
| [SetPrintPermission](./setprintpermission/) | Belgenin yazdırılmasına izin verilip verilmeyeceğini gösterir. |
| [GetModifyDocumentPermission](./getmodifydocumentpermission/) | AnnotationsPermission, FillFormsPermission ve AssembleDocumentPermission tarafından kontrol edilen işlemler dışındaki işlemlerle belgenin içeriğinin değiştirilmesine izin verilip verilmeyeceğini gösterir. |
| [SetModifyDocumentPermission](./setmodifydocumentpermission/) | AnnotationsPermission, FillFormsPermission ve AssembleDocumentPermission tarafından kontrol edilen işlemler dışındaki işlemlerle belgenin içeriğinin değiştirilmesine izin verilip verilmeyeceğini gösterir. |
| [GetAnnotationsPermission](./getannotationspermission/) | Metin açıklamaları eklemeye veya değiştirmeye, etkileşimli form alanlarını doldurmaya izin verilip verilmeyeceğini gösterir. |
| [SetAnnotationsPermission](./setannotationspermission/) | Metin açıklamaları eklemeye veya değiştirmeye, etkileşimli form alanlarını doldurmaya izin verilip verilmeyeceğini gösterir. |
| [GetFillFormsPermission](./getfillformspermission/) | ModifyDocumentPermission temiz olsa bile, mevcut etkileşimli form alanlarını (imza alanları dahil) doldurmaya izin verilip verilmeyeceğini gösterir. |
| [SetFillFormsPermission](./setfillformspermission/) | ModifyDocumentPermission temiz olsa bile, mevcut etkileşimli form alanlarını (imza alanları dahil) doldurmaya izin verilip verilmeyeceğini gösterir. |
| [GetExtractContentPermission](./getextractcontentpermission/) | AccessibilityExtractContent tarafından kontrol edilen işlemler dışındaki işlemlerle belgeden metin ve grafik kopyalamaya veya çıkarmaya izin verilip verilmeyeceğini gösterir. |
| [SetExtractContentPermission](./setextractcontentpermission/) | AccessibilityExtractContent tarafından kontrol edilen işlemler dışındaki işlemlerle belgeden metin ve grafik kopyalamaya veya çıkarmaya izin verilip verilmeyeceğini gösterir. |
| [GetAccessibilityExtractContent](./getaccessibilityextractcontent/) | Engelli kullanıcılar için erişilebilirliği desteklemek veya diğer amaçlarla metin ve grafik çıkarmaya izin verilip verilmeyeceğini gösterir. |
| [SetAccessibilityExtractContent](./setaccessibilityextractcontent/) | Engelli kullanıcılar için erişilebilirliği desteklemek veya diğer amaçlarla metin ve grafik çıkarmaya izin verilip verilmeyeceğini gösterir. |
| [GetAssembleDocumentPermission](./getassembledocumentpermission/) | ModifyDocumentPermission temiz olsa bile, belgeyi (sayfaları ekleme, döndürme veya silme ve yer imleri veya küçük resimler oluşturma) birleştirmeye izin verilip verilmeyeceğini gösterir. |
| [SetAssembleDocumentPermission](./setassembledocumentpermission/) | ModifyDocumentPermission temiz olsa bile, belgeyi (sayfaları ekleme, döndürme veya silme ve yer imleri veya küçük resimler oluşturma) birleştirmeye izin verilip verilmeyeceğini gösterir. |
| [GetFullQualityPrintPermission](./getfullqualityprintpermission/) | PDF içeriğinin doğru bir dijital kopyasının oluşturulabileceği bir temsile belgeyi yazdırmaya izin verilip verilmeyeceğini gösterir. |
| [SetFullQualityPrintPermission](./setfullqualityprintpermission/) | PDF içeriğinin doğru bir dijital kopyasının oluşturulabileceği bir temsile belgeyi yazdırmaya izin verilip verilmeyeceğini gösterir. |
