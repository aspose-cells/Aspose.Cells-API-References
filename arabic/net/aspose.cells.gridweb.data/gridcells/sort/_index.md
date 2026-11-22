---
title: "GridCells.Sort"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridCells. فرز البيانات تصاعديًا/تنازليًا من أعلى إلى أسفل في نطاق ورقة عمل حسب فهرس العمود المحدد. فرز البيانات تصاعديًا/تنازليًا من اليسار إلى اليمين في نطاق ورقة عمل حسب فهرس الصف المحدد"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridcells/sort/
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
 GridWeb GridWeb1 = new GridWeb();
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### انظر أيضًا

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_1}

يرتب البيانات تصاعديًا/تنازليًا من أعلى إلى أسفل في نطاق ورقة عمل حسب فهرس العمود المحدد. يرتب البيانات تصاعديًا/تنازليًا من اليسار إلى اليمين في نطاق ورقة عمل حسب فهرس الصف المحدد.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortByOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | رقم الصف للخلية الأولى للفرز. |
| startColumn | Int32 | رقم العمود للخلية الأولى للترتيب. |
| صفوف | Int32 | عدد الصفوف التي سيتم استيرادها. |
| أعمدة | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| فهارس | Int32[] | مصفوفة فهارس الأعمدة التي تحدد عمود الفرز. إذا كان الاتجاه من أعلى إلى أسفل، فإنها تمثل فهرس العمود الذي يحدد عمود الفرز. إذا كان الاتجاه من اليسار إلى اليمين، فإنها تمثل فهرس الصف الذي يحدد صف الفرز. |
| ترتيبات | SortByOrder[] | مصفوفة ترتيب الفرز. |
| الاتجاه | SortOrientation | اتجاه الفرز |
| isCaseSensitive | منطقي | ما إذا كان الفرز حساسًا لحالة الأحرف. |

### أمثلة

```csharp

 [C#]
 GridWeb GridWeb1=new GridWeb();
 int[] ids={0,1};
 SortByOrder[] sorder={SortByOrder.Ascending,SortByOrder.Descending};
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false);

 [VB]

 GridWeb1.WorkSheets(0).Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false)

```

### انظر أيضًا

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


