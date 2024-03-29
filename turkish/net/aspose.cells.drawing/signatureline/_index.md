---
title: SignatureLine
second_title: Aspose.Cells for .NET API Referansı
description: İmza satırını temsil eder.
type: docs
weight: 2770
url: /tr/net/aspose.cells.drawing/signatureline/
---
## SignatureLine class

İmza satırını temsil eder.

```csharp
public class SignatureLine
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [SignatureLine](signatureline)() | Default_Constructor |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AllowComments](../../aspose.cells.drawing/signatureline/allowcomments) { get; set; } | Yorumların eklenip eklenemeyeceğini gösterir. |
| [Email](../../aspose.cells.drawing/signatureline/email) { get; set; } | Şarkıcının e-postasını alır ve ayarlar. |
| [Id](../../aspose.cells.drawing/signatureline/id) { get; set; } | Bu imza satırı için tanımlayıcıyı alır veya ayarlar. |
| [Instructions](../../aspose.cells.drawing/signatureline/instructions) { get; set; } | İmzalama sırasında kullanıcıya gösterilen metni alır ve ayarlar. |
| [IsLine](../../aspose.cells.drawing/signatureline/isline) { get; set; } | İmza satırı olup olmadığını gösterir. |
| [ProviderId](../../aspose.cells.drawing/signatureline/providerid) { get; set; } | İmza sağlayıcısının kimliğini alır ve ayarlar. |
| [ShowSignedDate](../../aspose.cells.drawing/signatureline/showsigneddate) { get; set; } | İmzalı tarihin gösterilip gösterilmeyeceğini belirtir. |
| [Signer](../../aspose.cells.drawing/signatureline/signer) { get; set; } | İmzalayanı alır ve ayarlar. |
| [Title](../../aspose.cells.drawing/signatureline/title) { get; set; } | Şarkıcı unvanını alır ve ayarlar. |

### Örnekler

```csharp

[C#]

//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];

//Resim ekleme
int imgIndex = worksheet.Pictures.Add(1, 1, "sample.png");
Picture pic = worksheet.Pictures[imgIndex];
// İmza satırı nesnesi oluştur
SignatureLine s = new SignatureLine();
s.Signer = "Simon Zhao";
s.Title = "Development Lead";
s.Email = "Simon.Zhao@aspose.com";
// İmza satırı nesnesini Picture.SignatureLine özelliğine atayın
pic.SignatureLine = s;

//işini yap

//Excel dosyasını kaydedin.
workbook.Save("result.xlsx");
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
