---
title: "GridValidationCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridValidationCollection. أضف GridValidation إلى المجموعة. يتم تطبيق التحقق على الخلية المحددة."
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridvalidationcollection/add/
---
## Add(string) {#add_1}

أضف [`GridValidation`](../../gridvalidation/) إلى المجموعة. يتم تطبيق التحقق على الخلية المحددة.

```csharp
public GridValidation Add(string cellname)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellname | String | اسم الخلية. |

### قيمة الإرجاع

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### انظر أيضًا

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int) {#add}

أضف [`GridValidation`](../../gridvalidation/) إلى المجموعة. يتم تطبيق التحقق على الخلية المحددة.

```csharp
public GridValidation Add(int row, int col)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف للخلية. |
| عمود | Int32 | فهرس العمود للخلية. |

### قيمة الإرجاع

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### انظر أيضًا

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, bool, string) {#add_5}

يضيف تحققًا إلى خلية محددة باسم الخلية.

```csharp
public void Add(string cellName, bool isRequired, string regEx)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم خلية الشبكة. |
| isRequired | منطقي | قيمة تشير إلى ما إذا كانت قيمة الخلية مطلوبة. |
| regEx | String | تعبير نمطي. |

### انظر أيضًا

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, ICustomValidation) {#add_2}

يضيف تحققًا إلى خلية محددة عند فهرس الصف والعمود.

```csharp
public void Add(int row, int col, ICustomValidation customValidation)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف للخلية. |
| عمود | Int32 | فهرس العمود للخلية. |
| customValidation | ICustomValidation | كائن التحقق المخصص. |

### انظر أيضًا

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, bool, string) {#add_3}

يضيف تحققًا إلى خلية محددة عند فهرس الصف والعمود.

```csharp
public void Add(int row, int col, bool isRequired, string regEx)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف للخلية. |
| عمود | Int32 | فهرس العمود للخلية. |
| isRequired | منطقي | قيمة تشير إلى ما إذا كانت قيمة الخلية مطلوبة. |
| regEx | String | تعبير نمطي. |

### انظر أيضًا

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, ICustomValidation) {#add_4}

يضيف تحققًا إلى خلية محددة باسم الخلية.

```csharp
public void Add(string cellName, ICustomValidation customValidation)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم خلية الشبكة. |
| customValidation | ICustomValidation | كائن التحقق المخصص. |

### انظر أيضًا

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


