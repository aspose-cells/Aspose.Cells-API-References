---
title: SignatureLine
second_title: Aspose.Cells لمرجع .NET API
description: يمثل سطر التوقيع.
type: docs
weight: 2770
url: /ar/net/aspose.cells.drawing/signatureline/
---
## SignatureLine class

يمثل سطر التوقيع.

```csharp
public class SignatureLine
```

## المنشئون

| اسم | وصف |
| --- | --- |
| [SignatureLine](signatureline)() | Default_Constructor |

## الخصائص

| اسم | وصف |
| --- | --- |
| [AllowComments](../../aspose.cells.drawing/signatureline/allowcomments) { get; set; } | يشير إلى إمكانية إرفاق التعليقات. |
| [Email](../../aspose.cells.drawing/signatureline/email) { get; set; } | الحصول على البريد الإلكتروني للمغني وتعيينه. |
| [Id](../../aspose.cells.drawing/signatureline/id) { get; set; } | الحصول على أو تعيين معرف لسطر التوقيع هذا. |
| [Instructions](../../aspose.cells.drawing/signatureline/instructions) { get; set; } | الحصول على النص المعروض للمستخدم في وقت التوقيع وتعيينه. |
| [IsLine](../../aspose.cells.drawing/signatureline/isline) { get; set; } | يشير إلى ما إذا كان سطر توقيع. |
| [ProviderId](../../aspose.cells.drawing/signatureline/providerid) { get; set; } | الحصول على معرف موفر التوقيع وتعيينه. |
| [ShowSignedDate](../../aspose.cells.drawing/signatureline/showsigneddate) { get; set; } | يشير إلى ما إذا كان إظهار التاريخ الموقع. |
| [Signer](../../aspose.cells.drawing/signatureline/signer) { get; set; } | الحصول على الموقع وتعيينه . |
| [Title](../../aspose.cells.drawing/signatureline/title) { get; set; } | الحصول على عنوان المغني وتحديده . |

### أمثلة

```csharp

[C#]

// إنشاء كائن مصنف
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];

// إضافة صورة
int imgIndex = worksheet.Pictures.Add(1, 1, "sample.png");
Picture pic = worksheet.Pictures[imgIndex];
// إنشاء كائن سطر التوقيع
SignatureLine s = new SignatureLine();
s.Signer = "Simon Zhao";
s.Title = "Development Lead";
s.Email = "Simon.Zhao@aspose.com";
// تعيين كائن سطر التوقيع إلى خاصية Picture.SignatureLine
pic.SignatureLine = s;

// قم بعملك

// احفظ ملف Excel.
workbook.Save("result.xlsx");
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
