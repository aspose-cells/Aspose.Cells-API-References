---
title: "Класс DocumentProperty"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Properties.DocumentProperty class. Представляет пользовательское или встроенное свойство документа"
type: docs
url: /ru/net/aspose.cells.properties/documentproperty/
---
## DocumentProperty class

Представляет пользовательское или встроенное свойство документа.

```csharp
public class DocumentProperty
```

## Свойства

| Имя | Описание |
| --- | --- |
| [IsGeneratedName](../../aspose.cells.properties/documentproperty/isgeneratedname/) { get; } | Возвращает true, если у этого свойства нет имени в хранилище OLE2 и уникальное имя было сгенерировано только для публичного API. |
| [IsLinkedToContent](../../aspose.cells.properties/documentproperty/islinkedtocontent/) { get; } | Указывает, связано ли это свойство с содержимым |
| [Name](../../aspose.cells.properties/documentproperty/name/) { get; } | Возвращает имя свойства. |
| [Source](../../aspose.cells.properties/documentproperty/source/) { get; } | Связанный источник содержимого. |
| [Type](../../aspose.cells.properties/documentproperty/type/) { get; } | Получает тип данных свойства. |
| [Value](../../aspose.cells.properties/documentproperty/value/) { get; set; } | Получает или задает значение свойства. |

## Методы

| Имя | Описание |
| --- | --- |
| [ToBool](../../aspose.cells.properties/documentproperty/tobool/)() | Возвращает значение свойства как bool. |
| [ToDateTime](../../aspose.cells.properties/documentproperty/todatetime/)() | Возвращает значение свойства как DateTime в локальном часовом поясе. |
| [ToDouble](../../aspose.cells.properties/documentproperty/todouble/)() | Возвращает значение свойства как double. |
| [ToInt](../../aspose.cells.properties/documentproperty/toint/)() | Возвращает значение свойства как integer. |
| override [ToString](../../aspose.cells.properties/documentproperty/tostring/)() | Возвращает значение свойства как строку. |

### Примеры

```csharp

[C#]

//Создайте объект Workbook
Workbook workbook = new Workbook("book1.xls");
 
//Получите список всех пользовательских свойств документа Excel
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
//Получение пользовательского свойства документа с использованием индекса свойства
DocumentProperty customProperty1 = customProperties[3];
 
//Получение пользовательского свойства документа с использованием имени свойства
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

### См. также

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


