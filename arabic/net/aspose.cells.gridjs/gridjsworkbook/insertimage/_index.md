---
title: "GridJsWorkbook.InsertImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridJsWorkbook. إدراج صورة في ورقة العمل من تدفق ملف أو URL. يجب توفير إما تدفق الملف أو URL أو إدراج شكل عندما يكون p.type أحد AutoShapeType"
type: docs
url: /ar/net/aspose.cells.gridjs/gridjsworkbook/insertimage/
---
## GridJsWorkbook.InsertImage method

يدرج صورة في ورقة العمل من تدفق الملف أو URL (يجب توفير إما تدفق الملف أو URL) أو يدرج شكلًا عندما يكون p.type أحد AutoShapeType

```csharp
public string InsertImage(string uid, string p, Stream s, string imageUrl)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | String | المعرف الفريد لذاكرة التخزين المؤقت للملف |
| p | String | سلسلة تنسيق JSON للعملية التي تحدد موقع الخلية، اسم ورقة العمل، الصف العلوي الأيسر، العمود العلوي الأيسر للصورة، إلخ {name:'sheet1',ri:1,ci:1} |
| s | Stream | تدفق الملف لملف الصورة |
| imageUrl | String | عنوان URL لملف الصورة |

### قيمة الإرجاع

سلسلة تنسيق JSON للصورة المدخلة

### انظر أيضًا

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


