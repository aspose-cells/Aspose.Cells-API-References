---
title: CreateSubtotal
second_title: Aspose.Cells لمرجع .NET API
description: إنشاء المجموع الفرعي في الورقة .
type: docs
weight: 490
url: /ar/net/aspose.cells.gridweb.data/gridworksheet/createsubtotal/
---
## CreateSubtotal(int, int, int, SubtotalFunction, int[], string, GridTableItemStyle, GridTableItemStyle, NumberType, string) {#createsubtotal_1}

إنشاء المجموع الفرعي في الورقة .

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList, string functionLabel, 
    GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, NumberType numberType, 
    string customString)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| columnNameRowIndex | Int32 | فهرس الصف الخاص بصف اسم العمود. |
| dataRows | Int32 | عدد صفوف البيانات. |
| groupByColumnIndex | Int32 | فهرس العمود الخاص بالعمود المراد تجميعه. |
| subtotalFunction | SubtotalFunction | نوع دالة المجموع الفرعي. |
| subtotalColumnIndexList | Int32[] | فهارس الأعمدة المراد حصرها في المجموع الفرعي. |
| functionLabel | String | تسمية دالة المجموع الفرعي. |
| grandCellStyle | GridTableItemStyle | اسلوب الخط الكلي الكبير. |
| subtotalCellStyle | GridTableItemStyle | نمط خط المجموع الفرعي. |
| numberType | NumberType | نوع رقم خلايا نتيجة الإجمالي الفرعي. |
| customString | String | سلسلة تنسيق custome لخلايا نتيجة المجموع الفرعي. يمكن أن تكون خالية. |

### أنظر أيضا

* enum [SubtotalFunction](../../subtotalfunction)
* class [GridTableItemStyle](../../../aspose.cells.gridweb/gridtableitemstyle)
* enum [NumberType](../../numbertype)
* class [GridWorksheet](../../gridworksheet)
* مساحة الاسم [Aspose.Cells.GridWeb.Data](../../gridworksheet)
* المجسم [Aspose.Cells.GridWeb](../../../)

---

## CreateSubtotal(int, int, int, SubtotalFunction, int[]) {#createsubtotal}

إنشاء المجموع الفرعي في الورقة .

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| columnNameRowIndex | Int32 | فهرس الصف الخاص بصف اسم العمود. |
| dataRows | Int32 | عدد صفوف البيانات. |
| groupByColumnIndex | Int32 | فهرس العمود الخاص بالعمود المراد تجميعه. |
| subtotalFunction | SubtotalFunction | نوع دالة المجموع الفرعي. |
| subtotalColumnIndexList | Int32[] | فهارس الأعمدة المراد حصرها في المجموع الفرعي. |

### أنظر أيضا

* enum [SubtotalFunction](../../subtotalfunction)
* class [GridWorksheet](../../gridworksheet)
* مساحة الاسم [Aspose.Cells.GridWeb.Data](../../gridworksheet)
* المجسم [Aspose.Cells.GridWeb](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->