---
title: Replace
second_title: Aspose.Cells لمرجع .NET API
description: يستبدل قيمة الخلية بسلسلة جديدة.
type: docs
weight: 570
url: /ar/net/aspose.cells/workbook/replace/
---
## Replace(string, string) {#replace_7}

يستبدل قيمة الخلية بسلسلة جديدة.

```csharp
public int Replace(string placeHolder, string newValue)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| placeHolder | String | العنصر النائب للخلية |
| newValue | String | قيمة السلسلة المطلوب استبدالها |

### أمثلة

```csharp
[C#]

Workbook workbook = new Workbook();
......
workbook.Replace("AnOldValue", "NewValue");

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
 ........
orkbook.Replace("AnOldValue", "NewValue")
```

### أنظر أيضا

* class [Workbook](../../workbook)
* مساحة الاسم [Aspose.Cells](../../workbook)
* المجسم [Aspose.Cells](../../../)

---

## Replace(string, int) {#replace_4}

يستبدل قيمة الخلية بعدد صحيح جديد.

```csharp
public int Replace(string placeHolder, int newValue)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| placeHolder | String | العنصر النائب للخلية |
| newValue | Int32 | قيمة عدد صحيح لتحل محلها |

### أمثلة

```csharp
[C#]

Workbook workbook = new Workbook();
......
int newValue = 100;
workbook.Replace("AnOldValue", newValue);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
........
im NewValue As Integer =  100 
orkbook.Replace("AnOldValue", NewValue)
```

### أنظر أيضا

* class [Workbook](../../workbook)
* مساحة الاسم [Aspose.Cells](../../workbook)
* المجسم [Aspose.Cells](../../../)

---

## Replace(string, double) {#replace_2}

يستبدل قيمة الخلية بمزدوج جديد.

```csharp
public int Replace(string placeHolder, double newValue)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| placeHolder | String | العنصر النائب للخلية |
| newValue | Double | قيمة مزدوجة لتحل محلها |

### أمثلة

```csharp

[C#]

Workbook workbook = new Workbook();
......
double newValue = 100.0;
workbook.Replace("AnOldValue", newValue);


[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
........
im NewValue As Double =  100.0
orkbook.Replace("AnOldValue", NewValue)
```

### أنظر أيضا

* class [Workbook](../../workbook)
* مساحة الاسم [Aspose.Cells](../../workbook)
* المجسم [Aspose.Cells](../../../)

---

## Replace(string, string[], bool) {#replace_9}

يستبدل قيمة الخلية بمصفوفة سلسلة جديدة.

```csharp
public int Replace(string placeHolder, string[] newValues, bool isVertical)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| placeHolder | String | العنصر النائب للخلية |
| newValues | String[] | مجموعة سلسلة ليحل محلها |
| isVertical | Boolean | صحيح - عمودي ، خطأ - أفقي |

### أمثلة

```csharp

[C#]

Workbook workbook = new Workbook();
......
string[] newValues = new string[]{"Tom", "Alice", "Jerry"};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
.............
im NewValues() As String =  New String() {"Tom", "Alice", "Jerry"}		
orkbook.Replace("AnOldValue", NewValues, True)
```

### أنظر أيضا

* class [Workbook](../../workbook)
* مساحة الاسم [Aspose.Cells](../../workbook)
* المجسم [Aspose.Cells](../../../)

---

## Replace(string, int[], bool) {#replace_5}

يستبدل قيم الخلايا بمصفوفة عدد صحيح.

```csharp
public int Replace(string placeHolder, int[] newValues, bool isVertical)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| placeHolder | String | العنصر النائب للخلية |
| newValues | Int32[] | مجموعة عدد صحيح ليحل محل |
| isVertical | Boolean | صحيح - عمودي ، خطأ - أفقي |

### أمثلة

```csharp
[C#]

Workbook workbook = new Workbook();
......
int[] newValues = new int[]{1, 2, 3};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
..........
im NewValues() As Integer =  New Integer() {1, 2, 3}
orkbook.Replace("AnOldValue", NewValues, True)
```

### أنظر أيضا

* class [Workbook](../../workbook)
* مساحة الاسم [Aspose.Cells](../../workbook)
* المجسم [Aspose.Cells](../../../)

---

## Replace(string, double[], bool) {#replace_3}

يستبدل قيم الخلايا بمصفوفة مزدوجة.

```csharp
public int Replace(string placeHolder, double[] newValues, bool isVertical)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| placeHolder | String | العنصر النائب للخلية |
| newValues | Double[] | صفيف مزدوج ليحل محل |
| isVertical | Boolean | صحيح - عمودي ، خطأ - أفقي |

### أمثلة

```csharp

[C#]

Workbook workbook = new Workbook();
......
double[] newValues = new double[]{1.23, 2.56, 3.14159};
workbook.Replace("AnOldValue", newValues, true);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
...........
Dim NewValues() As Double =  New Double() {1.23, 2.56, 3.14159}
workbook.Replace("AnOldValue", NewValues, True)
```

### أنظر أيضا

* class [Workbook](../../workbook)
* مساحة الاسم [Aspose.Cells](../../workbook)
* المجسم [Aspose.Cells](../../../)

---

## Replace(string, DataTable) {#replace_6}

يستبدل قيم الخلايا ببيانات من ملفDataTable .

```csharp
public int Replace(string placeHolder, DataTable insertTable)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| placeHolder | String | العنصر النائب للخلية |
| insertTable | DataTable | يحل محل DataTable |

### أمثلة

```csharp
[C#]

Workbook workbook = new Workbook();
DataTable myDataTable = new DataTable("Customers");
// يضيف البيانات إلى myDataTable
........
workbook.Replace("AnOldValue", myDataTable);

[Visual Basic]

Dim workbook As Workbook =  New Workbook() 
Dim myDataTable As DataTable =  New DataTable("Customers") 
' يضيف البيانات إلى myDataTable
............
workbook.Replace("AnOldValue", myDataTable)
```

### أنظر أيضا

* class [Workbook](../../workbook)
* مساحة الاسم [Aspose.Cells](../../workbook)
* المجسم [Aspose.Cells](../../../)

---

## Replace(bool, object) {#replace}

يستبدل قيم الخلايا ببيانات جديدة.

```csharp
public int Replace(bool boolValue, object newValue)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| boolValue | Boolean | القيمة المنطقية المطلوب استبدالها. |
| newValue | Object | قيمة جديدة. يمكن أن تكون سلسلة أو عددًا صحيحًا أو مزدوجًا أو قيمة DateTime. |

### أنظر أيضا

* class [Workbook](../../workbook)
* مساحة الاسم [Aspose.Cells](../../workbook)
* المجسم [Aspose.Cells](../../../)

---

## Replace(int, object) {#replace_1}

يستبدل قيم الخلايا ببيانات جديدة.

```csharp
public int Replace(int intValue, object newValue)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| intValue | Int32 | القيمة الصحيحة المطلوب استبدالها. |
| newValue | Object | قيمة جديدة. يمكن أن تكون سلسلة أو عددًا صحيحًا أو مزدوجًا أو قيمة DateTime. |

### أنظر أيضا

* class [Workbook](../../workbook)
* مساحة الاسم [Aspose.Cells](../../workbook)
* المجسم [Aspose.Cells](../../../)

---

## Replace(string, string, ReplaceOptions) {#replace_8}

يستبدل قيمة الخلية بسلسلة جديدة.

```csharp
public int Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| placeHolder | String | العنصر النائب للخلية |
| newValue | String | قيمة السلسلة المطلوب استبدالها |
| options | ReplaceOptions | خيارات الاستبدال |

### أنظر أيضا

* class [ReplaceOptions](../../replaceoptions)
* class [Workbook](../../workbook)
* مساحة الاسم [Aspose.Cells](../../workbook)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
