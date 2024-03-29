---
title: Sort
second_title: Aspose.Cells لمرجع .NET API
description: يفرز البيانات تصاعديًا / تنازليًا من أعلى إلى أسفل في نطاق من ورقة العمل حسب فهرس العمود المحدد.
type: docs
weight: 740
url: /ar/net/aspose.cells.gridweb.data/gridcells/sort/
---
## Sort(int, int, int, int, int, bool, bool, bool) {#sort}

يفرز البيانات تصاعديًا / تنازليًا من أعلى إلى أسفل في نطاق من ورقة العمل حسب فهرس العمود المحدد.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, bool isAsending, 
    bool isCaseSensitive, bool islefttoright)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| startRow | Int32 | رقم صف الخلية الأولى المطلوب فرزها. |
| startColumn | Int32 | رقم العمود الخاص بالخلية الأولى المطلوب فرزها. |
| rows | Int32 | عدد الصفوف المراد استيرادها. |
| columns | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| index | Int32 | فهرس العمود الذي يحدد عمود الفرز. إذا كان الاتجاه من أعلى إلى أسفل ، فإنه يمثل فهرس العمود الذي يحدد عمود الفرز. صف. |
| isAsending | Boolean | ما إذا كان ترتيب الفرز متوقفًا. |
| isCaseSensitive | Boolean | ما إذا كان النوع حساسًا لحالة الأحرف. |
| islefttoright | Boolean | ما إذا كان اتجاه الفرز من اليسار إلى اليمين |

### أمثلة

```csharp

 [C#]

 GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### أنظر أيضا

* class [GridCells](../../gridcells)
* مساحة الاسم [Aspose.Cells.GridWeb.Data](../../gridcells)
* المجسم [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortOrder[], SortOrientation, bool) {#sort_1}

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

### أنظر أيضا

* enum [SortOrder](../../sortorder)
* enum [SortOrientation](../../sortorientation)
* class [GridCells](../../gridcells)
* مساحة الاسم [Aspose.Cells.GridWeb.Data](../../gridcells)
* المجسم [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
