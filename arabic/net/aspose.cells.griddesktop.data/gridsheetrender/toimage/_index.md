---
title: "GridSheetRender.ToImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "GridSheetRender طريقة. يرسم صفحة معينة إلى Graphics"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridsheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

عرض صفحة معينة إلى Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس الصفحة | Int32 | تحديد الصفحة التي سيتم تحويلها |
| g | الرسومات | الكائن الذي يتم الرسم إليه. |
| x | Single | إحداثي X (بالبيكسل) للزاوية العلوية اليسرى للصفحة المرسومة. |
| y | Single | إحداثي Y (بالبيكسل) للزاوية العلوية اليسرى للصفحة المرسومة. |
| العرض | Single | العرض الأقصى (بالبيكسل) الذي يمكن أن تشغله الصفحة المرسومة. |
| الارتفاع | Single | الارتفاع الأقصى (بالبيكسل) الذي يمكن أن تشغله الصفحة المرسومة. |

### انظر أيضًا

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

عرض صفحة معينة إلى Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس الصفحة | Int32 | تحديد الصفحة التي سيتم تحويلها |
| g | الرسومات | الكائن الذي يتم الرسم إليه. |
| x | Single | إحداثي X (بالبيكسل) للزاوية العلوية اليسرى للصفحة المرسومة. |
| y | Single | إحداثي Y (بالبيكسل) للزاوية العلوية اليسرى للصفحة المرسومة. |

### انظر أيضًا

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, string) {#toimage_4}

اعرض صفحة معينة إلى ملف.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس الصفحة | Int32 | تحديد الصفحة التي سيتم تحويلها |
| fileName | String | اسم ملف الصورة الناتجة |

### أمثلة

الكود التالي يُخرج الصفحة الأولى من الورقة الأولى إلى صورة png.

```csharp
//حمّل ملف المصدر مع الصور.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//تعيين نوع صورة الإخراج.
imgOpt.ImageType = ImageType.Png;

//عرض الورقة الأولى.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//إخراج الصفحة الأولى من الورقة إلى صورة.
sr.ToImage(0, "output.png");
```

### انظر أيضًا

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Stream) {#toimage_3}

اعرض صفحة معينة إلى تدفق.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس الصفحة | Int32 | تحديد الصفحة التي سيتم تحويلها |
| تدفق | Stream | تدفق الصورة الناتجة |

### انظر أيضًا

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int) {#toimage}

اعرض صفحة معينة إلى كائن Bitmap.

```csharp
public Bitmap ToImage(int pageIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس الصفحة | Int32 | تحديد الصفحة التي سيتم تحويلها |

### قيمة الإرجاع

كائن البت ماب للصفحة

### انظر أيضًا

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


