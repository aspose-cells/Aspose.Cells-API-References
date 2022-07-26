---
title: ConditionalFormattingCollection
second_title: Aspose.Cells لمرجع .NET API
description: لتغليف مجموعة منFormatCondition./formatcondition الكائنات .
type: docs
weight: 1100
url: /ar/net/aspose.cells/conditionalformattingcollection/
---
## ConditionalFormattingCollection class

لتغليف مجموعة من[`FormatCondition`](../formatcondition) الكائنات .

```csharp
public class ConditionalFormattingCollection : CollectionBase<FormatConditionCollection>
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingcollection/item) { get; } | يحصل على عنصر FormatConditions في الفهرس المحدد. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## طُرق

| اسم | وصف |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingcollection/add)() | يضيف "شروط التنسيق" إلى المجموعة. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(FormatConditionCollection) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(FormatConditionCollection) |  |
| [Copy](../../aspose.cells/conditionalformattingcollection/copy)(ConditionalFormattingCollection) | نسخ التنسيق الشرطي. |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(FormatConditionCollection[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(FormatConditionCollection[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, FormatConditionCollection[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(FormatConditionCollection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(FormatConditionCollection, int, int) |  |
| [RemoveArea](../../aspose.cells/conditionalformattingcollection/removearea)(int, int, int, int) | قم بإزالة كافة التنسيقات الشرطية في النطاق. |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### أمثلة

```csharp

[C#]

// إنشاء كائن مصنف
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

// احصل على تنسيق شرطي
ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;

// يضيف تنسيقًا شرطيًا فارغًا
int index = cformattings.Add();

// احصل على تنسيق شرطي مضاف حديثًا
FormatConditionCollection fcs = cformattings[index];

// يعين نطاق التنسيق الشرطي.
CellArea ca = new CellArea();

ca.StartRow = 0;

ca.EndRow = 0;

ca.StartColumn = 0;

ca.EndColumn = 0;

fcs.AddArea(ca);

ca = new CellArea();

ca.StartRow = 1;

ca.EndRow = 1;

ca.StartColumn = 1;

ca.EndColumn = 1;

fcs.AddArea(ca);

// إضافة شرط.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");

// إضافة شرط.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

// يعين لون الخلفية.
FormatCondition fc = fcs[conditionIndex];

fc.Style.BackgroundColor = Color.Red;

// حفظ ملف Excel
workbook.Save("output.xls");

[VB.NET]

'إنشاء كائن مصنف
DDim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'احصل على تنسيق شرطي
Dim cformattings As ConditionalFormattingCollection = sheet.ConditionalFormattings

'يضيف تنسيقًا شرطيًا فارغًا
Dim index As Integer = cformattings.Add()

'احصل على تنسيق شرطي مضاف حديثًا
Dim fcs As FormatConditionCollection = cformattings(index)

'يضبط نطاق التنسيق الشرطي.
Dim ca As New CellArea()

ca.StartRow = 0

ca.EndRow = 0

ca.StartColumn = 0

ca.EndColumn = 0

fcs.AddArea(ca)

ca = New CellArea()

ca.StartRow = 1

ca.EndRow = 1

ca.StartColumn = 1

ca.EndColumn = 1

fcs.AddArea(ca)

'أضف الشرط.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")

'أضف الشرط.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")

'يضبط لون الخلفية.
Dim fc As FormatCondition = fcs(conditionIndex)

fc.Style.BackgroundColor = Color.Red

'حفظ ملف Excel
workbook.Save("output.xls")
```

### أنظر أيضا

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [FormatConditionCollection](../formatconditioncollection)
* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
