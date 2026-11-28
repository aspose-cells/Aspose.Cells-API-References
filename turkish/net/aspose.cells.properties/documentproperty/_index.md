---
title: "Sınıf DocumentProperty"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Properties.DocumentProperty sınıfı. Özel veya yerleşik bir belge özelliğini temsil eder"
type: docs
url: /tr/net/aspose.cells.properties/documentproperty/
---
## DocumentProperty class

Özel veya yerleşik bir belge özelliğini temsil eder.

```csharp
public class DocumentProperty
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [IsGeneratedName](../../aspose.cells.properties/documentproperty/isgeneratedname/) { get; } | Bu özelliğin OLE2 depolamasında bir adı yoksa ve yalnızca genel API için benzersiz bir ad oluşturulduysa true döndürür. |
| [IsLinkedToContent](../../aspose.cells.properties/documentproperty/islinkedtocontent/) { get; } | Bu özelliğin içeriğe bağlı olup olmadığını gösterir |
| [Name](../../aspose.cells.properties/documentproperty/name/) { get; } | Özelliğin adını döndürür. |
| [Source](../../aspose.cells.properties/documentproperty/source/) { get; } | Bağlantılı içerik kaynağı. |
| [Type](../../aspose.cells.properties/documentproperty/type/) { get; } | Özelliğin veri tipini alır. |
| [Value](../../aspose.cells.properties/documentproperty/value/) { get; set; } | Özelliğin değerini alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ToBool](../../aspose.cells.properties/documentproperty/tobool/)() | Özellik değerini bool olarak döndürür. |
| [ToDateTime](../../aspose.cells.properties/documentproperty/todatetime/)() | Özellik değerini yerel saat diliminde DateTime olarak döndürür. |
| [ToDouble](../../aspose.cells.properties/documentproperty/todouble/)() | Özellik değerini double olarak döndürür. |
| [ToInt](../../aspose.cells.properties/documentproperty/toint/)() | Özellik değerini integer olarak döndürür. |
| override [ToString](../../aspose.cells.properties/documentproperty/tostring/)() | Özellik değerini string olarak döndürür. |

### Örnekler

```csharp

[C#]

//Bir Workbook nesnesi oluşturun
Workbook workbook = new Workbook("book1.xls");
 
//Excel dosyasının tüm özel belge özelliklerinin listesini al
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
//Özellik indeksini kullanarak bir özel belge özelliğine erişme
DocumentProperty customProperty1 = customProperties[3];
 
//Özellik adını kullanarak bir özel belge özelliğine erişme
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

### Ayrıca Bakınız

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


