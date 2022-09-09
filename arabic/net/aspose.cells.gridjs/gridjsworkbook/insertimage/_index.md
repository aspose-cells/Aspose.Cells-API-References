---
title: InsertImage
second_title: Aspose.Cells لمرجع .NET API
description: أدخل الصورة في ورقة العمل
type: docs
weight: 110
url: /ar/net/aspose.cells.gridjs/gridjsworkbook/insertimage/
---
## GridJsWorkbook.InsertImage method

أدخل الصورة في ورقة العمل

```csharp
public string InsertImage(string uid, string p, Stream s, string imageUrl)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| uid | String | المعرف الفريد لملف الورقة |
| p | String | حدد موقع الخلية ، تحتوي معلمة json على اسم الورقة والصف الأيسر العلوي والعمود الأيسر العلوي للصورة ， إلخ {name: 'sheet1'، ri: 1، ci: 1} |
| s | Stream | دفق ملف الصورة |
| imageUrl | String | عنوان url الخاص بملف الصورة ، إذا كانت imageUrl فارغة ، فسيتم حفظ الصورة في ذاكرة التخزين المؤقت ، وإلا فلن يتم حفظ الصورة |

### قيمة الإرجاع

json الصورة

### أنظر أيضا

* class [GridJsWorkbook](../../gridjsworkbook)
* مساحة الاسم [Aspose.Cells.GridJs](../../gridjsworkbook)
* المجسم [Aspose.Cells.GridJs](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridJs.dll -->