---
title: "WebCells.Sort"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WebCells. تقوم بترتيب البيانات تصاعديًا من أعلى إلى أسفل في نطاق من WebWorksheet حسب فهرس العمود المحدد"
type: docs
url: /ar/net/aspose.cells.gridweb.data/webcells/sort/
---
## Sort(int, int, int, int, int) {#sort}

يرتب البيانات تصاعديًا من الأعلى إلى الأسفل في نطاق WebWorksheet حسب فهرس العمود المحدد.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | رقم الصف للخلية الأولى للفرز. |
| startColumn | Int32 | رقم العمود للخلية الأولى للترتيب. |
| صفوف | Int32 | عدد الصفوف التي سيتم استيرادها. |
| أعمدة | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| فهرس | Int32 | فهرس العمود الذي يحدد عمود الفرز. |

### أمثلة

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3);

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3)

```

### انظر أيضًا

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int, SortByOrder, SortOrientation, bool) {#sort_1}

يرتب البيانات تصاعديًا من الأعلى إلى الأسفل في نطاق WebWorksheet حسب فهرس العمود المحدد.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, 
    SortByOrder sortOrder, SortOrientation sortOrientation, bool isCaseSensitive)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | رقم الصف للخلية الأولى للفرز. |
| startColumn | Int32 | رقم العمود للخلية الأولى للترتيب. |
| صفوف | Int32 | عدد الصفوف التي سيتم استيرادها. |
| أعمدة | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| فهرس | Int32 | فهرس العمود (أو الصف) الذي يحدد عمود (أو صف) الفرز. إذا كان اتجاه الفرز من أعلى إلى أسفل، فإن الفهرس يمثل فهرس العمود. إذا كان اتجاه الفرز من اليسار إلى اليمين، فإن الفهرس يمثل فهرس الصف. |
| ترتيب | SortByOrder | ترتيب الفرز: تصاعدي أو تنازلي |
| الاتجاه | SortOrientation | اتجاه الفرز: من أعلى إلى أسفل أو من اليسار إلى اليمين. |
| isCaseSensitive | منطقي | يشير إلى ما إذا كانت بيانات الفرز حساسة لحالة الأحرف إذا كانت البيانات نصية. |

### أمثلة

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,true)

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,True)

```

### انظر أيضًا

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[]) {#sort_2}

يرتب البيانات تصاعديًا من الأعلى إلى الأسفل في نطاق WebWorksheet حسب بعض الحقول المحددة بواسطة مصفوفة فهارس الأعمدة.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | رقم الصف للخلية الأولى للفرز. |
| startColumn | Int32 | رقم العمود للخلية الأولى للترتيب. |
| صفوف | Int32 | عدد الصفوف التي سيتم استيرادها. |
| أعمدة | Int32 | عدد الأعمدة التي سيتم استيرادها. |
| فهارس | Int32[] | مصفوفة فهارس الأعمدة التي تحدد البيانات التي يتم فرزها حسبها. |

### أمثلة

```csharp

[C#]

int[] indexes = new int[3];
indexes[0] = 0;
indexes[1] = 2;
indexes[2] = 3;
GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,indexes);

[VB]

Dim indexes() As Integer =  New Integer(3) {} 
indexes(0) = 0
indexes(1) = 2
indexes(2) = 3
GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,indexes)

```

### انظر أيضًا

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_3}

يرتب البيانات تصاعديًا في نطاق WebWorksheet حسب بعض الحقول المحددة بواسطة مصفوفة الفهارس.

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
| فهارس | Int32[] | فهرس العمود (أو الصف) الذي يحدد عمود (أو صف) الفرز. إذا كان اتجاه الفرز من أعلى إلى أسفل، فإن الفهرس يمثل فهرس العمود. إذا كان اتجاه الفرز من اليسار إلى اليمين، فإن الفهرس يمثل فهرس الصف. |
| ترتيبات | SortByOrder[] | ترتيب الفرز: تصاعدي أو تنازلي |
| الاتجاه | SortOrientation | اتجاه الفرز: من أعلى إلى أسفل أو من اليسار إلى اليمين. |
| isCaseSensitive | منطقي | يشير إلى ما إذا كان الفرز حساسًا لحالة الأحرف. |

### ملاحظات

إذا استخدمت هذه الطريقة لفرز كتلة من البيانات، يرجى التأكد من أن طول معامل الفهارس يساوي طول معامل الترتيب.

### أمثلة

```csharp

```

[C#] int[] indexes = new int[3]; indexes[0] = 0; indexes[1] = 1; indexes[2] = 3; SortOrder[] orders = new SortOrder[3]; orders[0] = SortOrder.Ascending; orders[1] = SortOrder.Descending; orders[2] = SortOrder.Descending; GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,false); [VB] Dim indexes() As Integer = New Integer(3) {} indexes(0) = 0 indexes(1) = 1 indexes(2) = 3 Dim orders() As SortOrder = New SortOrder(3) {} orders(0) = SortOrder.Ascending orders(1) = SortOrder.Descending orders(2) = SortOrder.Descending GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,False)

### انظر أيضًا

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


