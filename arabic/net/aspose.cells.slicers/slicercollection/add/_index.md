---
title: Add
second_title: Aspose.Cells لمرجع .NET API
description: إضافة أداة تقطيع جديدة باستخدام PivotTable كمصدر بيانات
type: docs
weight: 20
url: /ar/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

إضافة أداة تقطيع جديدة باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pivot | PivotTable | كائن PivotTable |
| destCellName | String | الخلية الموجودة في الزاوية العلوية اليسرى من نطاق مقسم طريقة العرض. |
| baseFieldName | String | اسم PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

إضافة فهرس القطاعة الجديد

### أمثلة

```csharp

[C#]

slicers.Add(pivot, "E3", "fruit");
```

### أنظر أيضا

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* مساحة الاسم [Aspose.Cells.Slicers](../../slicercollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

إضافة أداة تقطيع جديدة باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pivot | PivotTable | كائن PivotTable |
| row | Int32 | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق أداة تقطيع الشرائح. |
| column | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق القطاعة. |
| baseFieldName | String | اسم PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

إضافة فهرس القطاعة الجديد

### أمثلة

```csharp

[C#]

slicers.Add(pivot, 20, 12, "fruit");
```

### أنظر أيضا

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* مساحة الاسم [Aspose.Cells.Slicers](../../slicercollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

إضافة أداة تقطيع جديدة باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pivot | PivotTable | كائن PivotTable |
| row | Int32 | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق أداة تقطيع الشرائح. |
| column | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق القطاعة. |
| baseFieldIndex | Int32 | فهرس PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

إضافة فهرس القطاعة الجديد

### أمثلة

```csharp

[C#]

slicers.Add(pivot, 20, 8, 0);
```

### أنظر أيضا

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* مساحة الاسم [Aspose.Cells.Slicers](../../slicercollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

إضافة أداة تقطيع جديدة باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pivot | PivotTable | كائن PivotTable |
| destCellName | String | الخلية الموجودة في الزاوية العلوية اليسرى من نطاق مقسم طريقة العرض. |
| baseFieldIndex | Int32 | فهرس PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

إضافة فهرس القطاعة الجديد

### أمثلة

```csharp

[C#]

slicers.Add(pivot, "E20", 0);
```

### أنظر أيضا

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* مساحة الاسم [Aspose.Cells.Slicers](../../slicercollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

إضافة أداة تقطيع جديدة باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pivot | PivotTable | كائن PivotTable |
| row | Int32 | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق أداة تقطيع الشرائح. |
| column | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق القطاعة. |
| baseField | PivotField | PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

إضافة فهرس القطاعة الجديد

### أمثلة

```csharp

[C#]

slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
```

### أنظر أيضا

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* مساحة الاسم [Aspose.Cells.Slicers](../../slicercollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

إضافة أداة تقطيع جديدة باستخدام PivotTable كمصدر بيانات

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pivot | PivotTable | كائن PivotTable |
| destCellName | String | الخلية الموجودة في الزاوية العلوية اليسرى من نطاق مقسم طريقة العرض. |
| baseField | PivotField | PivotField في PivotTable.BaseFields |

### قيمة الإرجاع

إضافة فهرس القطاعة الجديد

### أمثلة

```csharp

[C#]

slicers.Add(pivot, "I3", pivot.BaseFields[0]);
```

### أنظر أيضا

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* مساحة الاسم [Aspose.Cells.Slicers](../../slicercollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

إضافة أداة تقطيع جديدة باستخدام ListObjet كمصدر بيانات

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| table | ListObject | كائن ListObject |
| index | Int32 | فهرس ListColumn في ListObject.ListColumns |
| destCellName | String | الخلية الموجودة في الزاوية العلوية اليسرى من نطاق مقسم طريقة العرض. |

### قيمة الإرجاع

إضافة فهرس القطاعة الجديد

### أمثلة

```csharp

[C#]

slicers.Add(table, 1, "E38");
```

### أنظر أيضا

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [SlicerCollection](../../slicercollection)
* مساحة الاسم [Aspose.Cells.Slicers](../../slicercollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

إضافة أداة تقطيع جديدة باستخدام ListObjet كمصدر بيانات

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| table | ListObject | كائن ListObject |
| listColumn | ListColumn | يعد ListColumn في ListObject.ListColumns |
| destCellName | String | الخلية الموجودة في الزاوية العلوية اليسرى من نطاق مقسم طريقة العرض. |

### قيمة الإرجاع

إضافة فهرس القطاعة الجديد

### أمثلة

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], "I38");
```

### أنظر أيضا

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* مساحة الاسم [Aspose.Cells.Slicers](../../slicercollection)
* المجسم [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

إضافة أداة تقطيع جديدة باستخدام ListObjet كمصدر بيانات

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| table | ListObject | كائن ListObject |
| listColumn | ListColumn | يعد ListColumn في ListObject.ListColumns |
| row | Int32 | فهرس صف الخلية في الزاوية العلوية اليسرى من نطاق أداة تقطيع الشرائح. |
| column | Int32 | فهرس العمود للخلية في الزاوية العلوية اليسرى من نطاق القطاعة. |

### قيمة الإرجاع

إضافة فهرس القطاعة الجديد

### أمثلة

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], 38, 12);
```

### أنظر أيضا

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* مساحة الاسم [Aspose.Cells.Slicers](../../slicercollection)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
