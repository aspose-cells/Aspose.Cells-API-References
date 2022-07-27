---
title: ConditionalFormattingIconCollection
second_title: Aspose.Cells لمرجع .NET API
description: يمثل مجموعة منConditionalFormattingIcon./conditionalformattingicon الكائنات .
type: docs
weight: 1120
url: /ar/net/aspose.cells/conditionalformattingiconcollection/
---
## ConditionalFormattingIconCollection class

يمثل مجموعة من[`ConditionalFormattingIcon`](../conditionalformattingicon) الكائنات .

```csharp
public class ConditionalFormattingIconCollection : CollectionBase<ConditionalFormattingIcon>
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingiconcollection/item) { get; } | الحصول على عنصر ConditionalFormattingIcon بالفهرس المحدد. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## طُرق

| اسم | وصف |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add#add)(ConditionalFormattingIcon) | يضيف[`ConditionalFormattingIcon`](../conditionalformattingicon) الكائن . |
| [Add](../../aspose.cells/conditionalformattingiconcollection/add#add_1)(IconSetType, int) | يضيف[`ConditionalFormattingIcon`](../conditionalformattingicon) الكائن . |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(ConditionalFormattingIcon) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(ConditionalFormattingIcon, IComparer&lt;ConditionalFormattingIcon&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, ConditionalFormattingIcon, IComparer&lt;ConditionalFormattingIcon&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(ConditionalFormattingIcon) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(ConditionalFormattingIcon[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(ConditionalFormattingIcon[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, ConditionalFormattingIcon[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;ConditionalFormattingIcon&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ConditionalFormattingIcon) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ConditionalFormattingIcon, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ConditionalFormattingIcon, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ConditionalFormattingIcon) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ConditionalFormattingIcon, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ConditionalFormattingIcon, int, int) |  |
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

// يعين الشرط
 int idx = fcs.AddCondition(FormatConditionType.IconSet);
 
 FormatCondition cond = fcs[idx];
   
 // يعين الشرط's type
 cond.IconSet.Type = IconSetType.ArrowsGray3;

// إضافة حالة رموز مخصصة.
 ConditionalFormattingIcon cfIcon = cond.IconSet.CfIcons[0];
 
 cfIcon.Type = IconSetType.Arrows3;
 
 cfIcon.Index = 0;
 
 ConditionalFormattingIcon cfIcon1 = cond.IconSet.CfIcons[1];
 
  cfIcon1.Type = IconSetType.ArrowsGray3;
  
  cfIcon1.Index = 1;
  
  ConditionalFormattingIcon cfIcon2 = cond.IconSet.CfIcons[2];
  
  cfIcon2.Type = IconSetType.Boxes5;
  
  cfIcon2.Index = 2;

// حفظ ملف Excel
workbook.Save("output.xls");

[VB.NET]

'إنشاء كائن مصنف
Dim workbook As Workbook = New Workbook()

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

// يعين الشرط
Dim idx As Integer =fcs.AddCondition(FormatConditionType.IconSet)

Dim cond As FormatCondition=fcs[idx]

// يعين الشرط's type
cfIcon.Type = IconSetType.ArrowsGray3

'إضافة حالة رموز مخصصة.
Dim cfIcon As ConditionalFormattingIcon = cond.IconSet.CfIcons[0]

cfIcon.Type = IconSetType.Arrows3

cfIcon.Index=0

Dim cfIcon1 As ConditionalFormattingIcon = cond.IconSet.CfIcons[1]

cfIcon1.Type = IconSetType.ArrowsGray3

cfIcon1.Index=1

Dim cfIcon2 As ConditionalFormattingIcon = cond.IconSet.CfIcons[2]

cfIcon2.Type = IconSetType.Boxes5

cfIcon2.Index=2

'حفظ ملف Excel
workbook.Save("output.xls")
```

### أنظر أيضا

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [ConditionalFormattingIcon](../conditionalformattingicon)
* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
