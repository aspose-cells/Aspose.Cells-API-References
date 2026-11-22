---
title: "GridHyperlinkCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridHyperlinkCollection. يضيف رابطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridhyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | الصف الأول من نطاق الارتباط التشعبي. |
| firstColumn | Int32 | العمود الأول من نطاق الارتباط التشعبي. |
| totalRows | Int32 | عدد الصفوف في هذا النطاق التشعبي. |
| totalColumns | Int32 | عدد الأعمدة في هذا النطاق التشعبي. |
| address | String | عنوان الارتباط التشعبي. |

### قيمة الإرجاع

فهرس كائن الارتباط التشعبي.

### أمثلة

```csharp
[C#]

Worksheet worksheet = excel.Worksheets[0];
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com");
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls");

[Visual Basic]

Dim worksheet as Worksheet = excel.Worksheets(0)
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com")
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls")

```

### انظر أيضًا

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, int, int, string) {#add_1}

يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم الخلية. |
| totalRows | Int32 | عدد الصفوف في هذا النطاق التشعبي. |
| totalColumns | Int32 | عدد الأعمدة في هذا النطاق التشعبي. |
| address | String | عنوان الارتباط التشعبي. |

### قيمة الإرجاع

فهرس كائن الارتباط التشعبي.

### انظر أيضًا

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, string) {#add_2}

يضيف ارتباطًا تشعبيًا إلى خلية محددة.

```csharp
public int Add(string cellName, string address)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم الخلية. |
| address | String | عنوان الارتباط التشعبي. |

### قيمة الإرجاع

فهرس كائن الارتباط التشعبي.

### انظر أيضًا

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, string, string, string, string) {#add_3}

يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startCellName | String | الخلية العلوية اليسرى للنطاق. |
| endCellName | String | الخلية السفلية اليمنى للنطاق. |
| address | String | عنوان الارتباط التشعبي. |
| textToDisplay | String | النص الذي سيتم عرضه للارتباط التشعبي المحدد. |
| screenTip | String | نص الـ screenTip للارتباط التشعبي المحدد. |

### قيمة الإرجاع

فهرس كائن الارتباط التشعبي.

### انظر أيضًا

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, string) {#add_4}

يضيف ارتباطًا تشعبيًا إلى خلية محددة في فهرس الصف والعمود.

```csharp
public void Add(int row, int col, string url)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف للخلية. |
| عمود | Int32 | فهرس العمود للخلية. |
| url | String | عنوان URL للارتباط التشعبي. |

### انظر أيضًا

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


