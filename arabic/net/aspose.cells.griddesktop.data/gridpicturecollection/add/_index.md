---
title: "GridPictureCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridPictureCollection. إضافة صورة إلى المجموعة"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridpicturecollection/add/
---
## Add(int, int, int, int, Stream) {#add}

يضيف صورة إلى المجموعة.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| upperLeftRow | Int32 | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | Int32 | فهرس العمود العلوي الأيسر. |
| lowerRightRow | Int32 | فهرس الصف السفلي الأيمن |
| lowerRightColumn | Int32 | فهرس العمود السفلي الأيمن |
| تدفق | Stream | كائن Stream الذي يحتوي على بيانات الصورة. |

### قيمة الإرجاع

فهرس كائن الصورة.

### انظر أيضًا

* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, int, int, string) {#add_1}

يضيف صورة إلى المجموعة.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn, 
    string fileName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| upperLeftRow | Int32 | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | Int32 | فهرس العمود العلوي الأيسر. |
| lowerRightRow | Int32 | فهرس الصف السفلي الأيمن |
| lowerRightColumn | Int32 | فهرس العمود السفلي الأيمن |
| fileName | String | اسم ملف الصورة. |

### قيمة الإرجاع

فهرس كائن الصورة.

### انظر أيضًا

* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, Stream) {#add_2}

يضيف صورة إلى المجموعة.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| upperLeftRow | Int32 | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | Int32 | فهرس العمود العلوي الأيسر. |
| تدفق | Stream | كائن Stream الذي يحتوي على بيانات الصورة. |

### قيمة الإرجاع

فهرس كائن الصورة.

### انظر أيضًا

* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, string) {#add_3}

يضيف صورة إلى المجموعة.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| upperLeftRow | Int32 | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | Int32 | فهرس العمود العلوي الأيسر. |
| fileName | String | اسم ملف الصورة. |

### قيمة الإرجاع

[`GridPicture`](../../gridpicture/) object index.

### انظر أيضًا

* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, string, int, int) {#add_4}

يضيف صورة إلى المجموعة.

```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName, int widthScale, 
    int heightScale)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| upperLeftRow | Int32 | فهرس الصف العلوي الأيسر. |
| upperLeftColumn | Int32 | فهرس العمود العلوي الأيسر. |
| fileName | String | اسم ملف الصورة. |
| widthScale | Int32 | مقياس عرض الصورة، نسبة مئوية. |
| heightScale | Int32 | مقياس ارتفاع الصورة، نسبة مئوية. |

### قيمة الإرجاع

[`GridPicture`](../../gridpicture/) object index.

### انظر أيضًا

* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, string) {#add_6}

يضيف صورة إلى خلية محددة باسم الخلية.

```csharp
public void Add(string cellName, string fileName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم خلية الشبكة. |
| fileName | String | اسم ملف الصورة. |

### انظر أيضًا

* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, Image) {#add_5}

يضيف صورة إلى خلية محددة بحسب فهرس الصف والعمود.

```csharp
public void Add(int row, int col, Image image)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف للخلية. |
| عمود | Int32 | فهرس العمود للخلية. |
| صورة | صورة | صورة. |

### انظر أيضًا

* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


