---
title: Add
second_title: Aspose.Cells لمرجع .NET API
description: إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات
type: docs
weight: 20
url: /ar/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pivot | PivotTable | كائن PivotTable |
| row | Int32 | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني. |
| column | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني. |
| baseFieldName | String | اسم PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

إضافة فهرس الجدول الزمني الجديد

### أمثلة

```csharp

[C#]
// إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات
sheet.Timelines.Add(pivot, 10, 5, "date");
```

### أنظر أيضا

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* مساحة الاسم [Aspose.Cells.Timelines](../../timelinecollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pivot | PivotTable | كائن PivotTable |
| destCellName | String | اسم الخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني. |
| baseFieldName | String | اسم PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

إضافة فهرس الجدول الزمني الجديد

### أمثلة

```csharp

[C#]
// إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات
sheet.Timelines.Add(pivot, "i15", "date");
```

### أنظر أيضا

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* مساحة الاسم [Aspose.Cells.Timelines](../../timelinecollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pivot | PivotTable | كائن PivotTable |
| row | Int32 | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني. |
| column | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني. |
| baseFieldIndex | Int32 | فهرس PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

إضافة فهرس الجدول الزمني الجديد

### أمثلة

```csharp

[C#]
// إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات
sheet.Timelines.Add(pivot, 15, 5, 1);
```

### أنظر أيضا

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* مساحة الاسم [Aspose.Cells.Timelines](../../timelinecollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pivot | PivotTable | كائن PivotTable |
| destCellName | String | اسم الخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني. |
| baseFieldIndex | Int32 | فهرس PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

إضافة فهرس الجدول الزمني الجديد

### أمثلة

```csharp

[C#]
// إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات
sheet.Timelines.Add(pivot, "i5", 1);
```

### أنظر أيضا

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* مساحة الاسم [Aspose.Cells.Timelines](../../timelinecollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pivot | PivotTable | كائن PivotTable |
| row | Int32 | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني. |
| column | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني. |
| baseField | PivotField | PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

إضافة فهرس الجدول الزمني الجديد

### أمثلة

```csharp

[C#]
// إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات
sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
```

### أنظر أيضا

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* مساحة الاسم [Aspose.Cells.Timelines](../../timelinecollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pivot | PivotTable | كائن PivotTable |
| destCellName | String | اسم الخلية في الزاوية العلوية اليسرى من نطاق المخطط الزمني. |
| baseField | PivotField | PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

إضافة فهرس الجدول الزمني الجديد

### أمثلة

```csharp

[C#]
// إضافة مخطط زمني جديد باستخدام PivotTable كمصدر بيانات
sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[1]);
```

### أنظر أيضا

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* مساحة الاسم [Aspose.Cells.Timelines](../../timelinecollection)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
