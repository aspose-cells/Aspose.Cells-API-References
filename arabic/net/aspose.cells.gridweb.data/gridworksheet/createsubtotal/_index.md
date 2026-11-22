---
title: "GridWorksheet.CreateSubtotal"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridWorksheet. إنشاء مجموع فرعي في الورقة"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridworksheet/createsubtotal/
---
## CreateSubtotal(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) {#createsubtotal_1}

ينشئ مجموعًا فرعيًا في الورقة.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList, string functionLabel, 
    GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, NumberType numberType, 
    string customString)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnNameRowIndex | Int32 | فهرس الصف لصف اسم العمود. |
| dataRows | Int32 | عدد صفوف البيانات. |
| groupByColumnIndex | Int32 | فهرس العمود للعمود الذي سيتم تجميعه. |
| subtotalFunction | SubtotalFunction | نوع دالة المجموع الفرعي. |
| subtotalColumnIndexList | Int32[] | مؤشرات الأعمدة التي سيتم جمعها فرعياً. |
| functionLabel | String | تسمية دالة المجموع الفرعي. |
| grandCellStyle | GridTableItemStyle | نمط سطر المجموع الكلي. |
| subtotalCellStyle | GridTableItemStyle | نمط سطر المجموع الفرعي. |
| numberType | NumberType | نوع الرقم لخلايا نتيجة المجموع الفرعي. |
| customString | String | سلسلة التنسيق المخصصة لخلايا نتيجة المجموع الفرعي. يمكن أن تكون فارغة. |

### انظر أيضًا

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridTableItemStyle](../../../aspose.cells.gridweb/gridtableitemstyle/)
* enum [NumberType](../../numbertype/)
* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreateSubtotal(int, int, int, SubtotalFunction, int[]) {#createsubtotal}

ينشئ مجموعًا فرعيًا في الورقة.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnNameRowIndex | Int32 | فهرس الصف لصف اسم العمود. |
| dataRows | Int32 | عدد صفوف البيانات. |
| groupByColumnIndex | Int32 | فهرس العمود للعمود الذي سيتم تجميعه. |
| subtotalFunction | SubtotalFunction | نوع دالة المجموع الفرعي. |
| subtotalColumnIndexList | Int32[] | مؤشرات الأعمدة التي سيتم جمعها فرعياً. |

### انظر أيضًا

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


