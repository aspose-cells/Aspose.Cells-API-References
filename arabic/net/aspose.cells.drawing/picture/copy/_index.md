---
title: Copy
second_title: Aspose.Cells لمرجع .NET API
description: انسخ الصورة .
type: docs
weight: 180
url: /ar/net/aspose.cells.drawing/picture/copy/
---
## Picture.Copy method

انسخ الصورة .

```csharp
public void Copy(Picture source, CopyOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| source | Picture | الصورة المصدر. |
| options | CopyOptions | خيارات النسخ. |

### أمثلة

```csharp

[C#]
// إنشاء كائن مصنف
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// أدخل الصورة الأولى
int imgIndex1 = worksheet.Pictures.Add(1, 1, "1.png");
// احصل على كائن الصورة المدرج
Picture pic1 = worksheet.Pictures[imgIndex1];
// أدخل الصورة الثانية
int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
// احصل على كائن الصورة المدرج
Picture pic2 = worksheet.Pictures[imgIndex2];
// نسخ الصورة 1 إلى الصورة 2. ستحصل على كائنين من الصورة 1 متراكبين فوق بعضهما البعض.
CopyOptions opt = new CopyOptions();
pic2.Copy(pic1, opt);
// احفظ ملف Excel.
workbook.Save("result.xlsx");
```

### أنظر أيضا

* class [CopyOptions](../../../aspose.cells/copyoptions)
* class [Picture](../../picture)
* مساحة الاسم [Aspose.Cells.Drawing](../../picture)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->