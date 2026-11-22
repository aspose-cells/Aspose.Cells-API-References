---
title: "الفئة DocumentProperty"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Properties.DocumentProperty class. يمثل خاصية مستند مخصصة أو مدمجة"
type: docs
url: /ar/net/aspose.cells.properties/documentproperty/
---
## DocumentProperty class

يمثل خاصية مستند مخصصة أو مدمجة.

```csharp
public class DocumentProperty
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [IsGeneratedName](../../aspose.cells.properties/documentproperty/isgeneratedname/) { get; } | يعيد true إذا لم يكن لهذه الخاصية اسم في تخزين OLE2 وتم إنشاء اسم فريد فقط لواجهة برمجة التطبيقات العامة. |
| [IsLinkedToContent](../../aspose.cells.properties/documentproperty/islinkedtocontent/) { get; } | يشير إلى ما إذا كانت هذه الخاصية مرتبطة بالمحتوى |
| [Name](../../aspose.cells.properties/documentproperty/name/) { get; } | يعيد اسم الخاصية. |
| [Source](../../aspose.cells.properties/documentproperty/source/) { get; } | مصدر المحتوى المرتبط. |
| [Type](../../aspose.cells.properties/documentproperty/type/) { get; } | يحصل على نوع البيانات للخاصية. |
| [Value](../../aspose.cells.properties/documentproperty/value/) { get; set; } | يحصل أو يعيّن قيمة الخاصية. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ToBool](../../aspose.cells.properties/documentproperty/tobool/)() | يعيد قيمة الخاصية كقيمة منطقية. |
| [ToDateTime](../../aspose.cells.properties/documentproperty/todatetime/)() | يعيد قيمة الخاصية كـ DateTime في المنطقة الزمنية المحلية. |
| [ToDouble](../../aspose.cells.properties/documentproperty/todouble/)() | يعيد قيمة الخاصية كقيمة مزدوجة. |
| [ToInt](../../aspose.cells.properties/documentproperty/toint/)() | يعيد قيمة الخاصية كعدد صحيح. |
| override [ToString](../../aspose.cells.properties/documentproperty/tostring/)() | يعيد قيمة الخاصية كسلسلة نصية. |

### أمثلة

```csharp

[C#]

//إنشاء كائن Workbook
Workbook workbook = new Workbook("book1.xls");
 
//استرجاع قائمة بجميع الخصائص الموثقة المخصصة لملف Excel
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
//الوصول إلى خاصية مستند مخصصة باستخدام فهرس الخاصية
DocumentProperty customProperty1 = customProperties[3];
 
//الوصول إلى خاصية مستند مخصصة باستخدام اسم الخاصية
DocumentProperty customProperty2 = customProperties["Owner"];

[VB.NET]

'Instantiate a Workbook object
Dim workbook As Workbook = New Workbook("book1.xls")
 
'Retrieve a list of all custom document properties of the Excel file
Dim customProperties As DocumentPropertyCollection = workbook.Worksheets.CustomDocumentProperties
 
'Accessng a custom document property by using the property index
Dim customProperty1 As DocumentProperty = customProperties(3)
 
'Accessng a custom document property by using the property name
Dim customProperty2 As DocumentProperty = customProperties("Owner")
```

### انظر أيضًا

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


