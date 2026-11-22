---
title: "GridCells.Sort"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridCells. فرز البيانات تصاعديًا/تنازليًا من أعلى إلى أسفل في نطاق ورقة عمل حسب فهرس العمود المحدد. فرز البيانات تصاعديًا/تنازليًا من اليسار إلى اليمين في نطاق ورقة عمل حسب فهرس الصف المحدد"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridcells/sort/
---
## Sort(int, int, int, int, int, bool, bool, bool) {#sort}

يرتب البيانات تصاعديًا/تنازليًا من أعلى إلى أسفل في نطاق ورقة عمل حسب فهرس العمود المحدد. يرتب البيانات تصاعديًا/تنازليًا من اليسار إلى اليمين في نطاق ورقة عمل حسب فهرس الصف المحدد.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, bool isAsending, 
    bool isCaseSensitive, bool islefttoright)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | رقم الصف للخلية الأولى للفرز. |
| startColumn | Int32 | رقم العمود للخلية الأولى للترتيب. |
| صفوف | Int32 | عدد الصفوف التي سيتم استيرادها. |
| أعمدة | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| فهرس | Int32 | مؤشر العمود الذي يحدد عمود الفرز. إذا كان الاتجاه من الأعلى إلى الأسفل، فهو يمثل مؤشر العمود الذي يحدد عمود الفرز. إذا كان الاتجاه من اليسار إلى اليمين، فهو يمثل مؤشر الصف الذي يحدد صف الفرز. |
| isAsending | منطقي | ما إذا كان ترتيب الفرز تصاعديًا. |
| isCaseSensitive | منطقي | ما إذا كان الفرز حساسًا لحالة الأحرف. |
| islefttoright | منطقي | ما إذا كان اتجاه الفرز من اليسار إلى اليمين |

### أمثلة

```csharp

 [C#]

 GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### انظر أيضًا

* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Sort(int, int, int, int, int[], SortOrder[], SortOrientation, bool) {#sort_1}

يرتب بيانات المنطقة.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| معامل | الوصف |
| --- | --- |
| الخلايا | الخلايا تحتوي على منطقة البيانات. |
| startRow | صف البداية للمنطقة. |
| startColumn | عمود البداية للمنطقة. |
| صفوف | إجمالي الصفوف. |
| أعمدة | إجمالي الأعمدة. |
| فهارس | مصفوفة مؤشرات الأعمدة المرتبة |
| ترتيبات | مصفوفة ترتيب الفرز |
| الاتجاه | اتجاه الفرز: من اليسار إلى اليمين أو من الأعلى إلى الأسفل. |
| isCaseSensitive | ما إذا كان حساسًا لحالة الأحرف عند مقارنة السلاسل. |

### انظر أيضًا

* enum [SortOrder](../../../aspose.cells.griddesktop/sortorder/)
* enum [SortOrientation](../../../aspose.cells.griddesktop/sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


