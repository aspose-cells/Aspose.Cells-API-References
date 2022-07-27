---
title: Add
second_title: Aspose.Cells لمرجع .NET API
description: يضيف صورة إلى المجموعة.
type: docs
weight: 20
url: /ar/net/aspose.cells.drawing/picturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

يضيف صورة إلى المجموعة.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    Stream stream)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| upperLeftRow | Int32 | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | Int32 | فهرس العمود الأيسر العلوي. |
| lowerRightRow | Int32 | فهرس الصف السفلي الأيمن |
| lowerRightColumn | Int32 | فهرس العمود الأيمن السفلي |
| stream | Stream | كائن دفق يحتوي على بيانات الصورة. |

### قيمة الإرجاع

[`Picture`](../../picture) فهرس الكائن.

### أمثلة

```csharp

[C#]
// إضافة صورة
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, 5, 5, fs);
}
```

### أنظر أيضا

* class [PictureCollection](../../picturecollection)
* مساحة الاسم [Aspose.Cells.Drawing](../../picturecollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(int, int, int, int, string) {#add_1}

يضيف صورة إلى المجموعة.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    string fileName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| upperLeftRow | Int32 | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | Int32 | فهرس العمود الأيسر العلوي. |
| lowerRightRow | Int32 | فهرس الصف السفلي الأيمن |
| lowerRightColumn | Int32 | فهرس العمود الأيمن السفلي |
| fileName | String | اسم ملف الصورة. |

### قيمة الإرجاع

[`Picture`](../../picture) فهرس الكائن.

### أمثلة

```csharp

[C#]
// إضافة صورة
pictures.Add(1, 1, 5, 5, "image.jpg");
```

### أنظر أيضا

* class [PictureCollection](../../picturecollection)
* مساحة الاسم [Aspose.Cells.Drawing](../../picturecollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(int, int, Stream) {#add_2}

يضيف صورة إلى المجموعة.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| upperLeftRow | Int32 | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | Int32 | فهرس العمود الأيسر العلوي. |
| stream | Stream | كائن دفق يحتوي على بيانات الصورة. |

### قيمة الإرجاع

[`Picture`](../../picture) فهرس الكائن.

### أمثلة

```csharp

[C#]
// إضافة صورة
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs);
}
```

### أنظر أيضا

* class [PictureCollection](../../picturecollection)
* مساحة الاسم [Aspose.Cells.Drawing](../../picturecollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(int, int, string) {#add_4}

يضيف صورة إلى المجموعة.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| upperLeftRow | Int32 | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | Int32 | فهرس العمود الأيسر العلوي. |
| fileName | String | اسم ملف الصورة. |

### قيمة الإرجاع

[`Picture`](../../picture) فهرس الكائن.

### أمثلة

```csharp

[C#]
// إضافة صورة
pictures.Add(1, 1, "image.jpg");
```

### أنظر أيضا

* class [PictureCollection](../../picturecollection)
* مساحة الاسم [Aspose.Cells.Drawing](../../picturecollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(int, int, Stream, int, int) {#add_3}

يضيف صورة إلى المجموعة.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream, int widthScale, 
    int heightScale)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| upperLeftRow | Int32 | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | Int32 | فهرس العمود الأيسر العلوي. |
| stream | Stream | كائن دفق يحتوي على بيانات الصورة. |
| widthScale | Int32 | مقياس عرض الصورة ، نسبة مئوية. |
| heightScale | Int32 | مقياس ارتفاع الصورة ، نسبة مئوية. |

### قيمة الإرجاع

[`Picture`](../../picture) فهرس الكائن.

### أمثلة

```csharp

[C#]
// إضافة صورة
using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
{
    pictures.Add(1, 1, fs, 50, 50);
}
```

### أنظر أيضا

* class [PictureCollection](../../picturecollection)
* مساحة الاسم [Aspose.Cells.Drawing](../../picturecollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(int, int, string, int, int) {#add_5}

يضيف صورة إلى المجموعة.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName, int widthScale, 
    int heightScale)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| upperLeftRow | Int32 | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | Int32 | فهرس العمود الأيسر العلوي. |
| fileName | String | اسم ملف الصورة. |
| widthScale | Int32 | مقياس عرض الصورة ، نسبة مئوية. |
| heightScale | Int32 | مقياس ارتفاع الصورة ، نسبة مئوية. |

### قيمة الإرجاع

[`Picture`](../../picture) فهرس الكائن.

### أمثلة

```csharp

[C#]
// إضافة صورة
pictures.Add(1, 1, "image.jpg", 50, 50);
```

### أنظر أيضا

* class [PictureCollection](../../picturecollection)
* مساحة الاسم [Aspose.Cells.Drawing](../../picturecollection)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
