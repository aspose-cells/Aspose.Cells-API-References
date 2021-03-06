---
title: DocumentPropertyCollection
second_title: Справочник по Aspose.Cells для .NET API
description: Базовый класс дляBuiltInDocumentPropertyCollection./builtindocumentpropertycollectionиCustomDocumentPropertyCollection./customdocumentpropertycollectionколлекции.
type: docs
weight: 4870
url: /ru/net/aspose.cells.properties/documentpropertycollection/
---
## DocumentPropertyCollection class

Базовый класс для[`BuiltInDocumentPropertyCollection`](../builtindocumentpropertycollection)и[`CustomDocumentPropertyCollection`](../customdocumentpropertycollection)коллекции.

```csharp
public abstract class DocumentPropertyCollection : IEnumerable
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.cells.properties/documentpropertycollection/count) { get; } | Получает количество элементов в коллекции. |
| [Item](../../aspose.cells.properties/documentpropertycollection/item) { get; } | Возвращает объект[`DocumentProperty`](../documentproperty)по индексу. |
| virtual [Item](../../aspose.cells.properties/documentpropertycollection/item) { get; } | Возвращает объект[`DocumentProperty`](../documentproperty)по имени свойства. |

## Методы

| Имя | Описание |
| --- | --- |
| [Clear](../../aspose.cells.properties/documentpropertycollection/clear)() | Удаляет все свойства из коллекции. |
| [Contains](../../aspose.cells.properties/documentpropertycollection/contains)(string) | Возвращает true, если свойство с указанным именем существует в коллекции. |
| [GetEnumerator](../../aspose.cells.properties/documentpropertycollection/getenumerator)() |  |
| [IndexOf](../../aspose.cells.properties/documentpropertycollection/indexof)(string) | Получает индекс свойства по имени. |
| [Remove](../../aspose.cells.properties/documentpropertycollection/remove)(string) | Удаляет свойство с указанным именем из коллекции. |
| [RemoveAt](../../aspose.cells.properties/documentpropertycollection/removeat)(int) | Удаляет свойство по указанному индексу. |

### Примеры

```csharp

[C#]

  //Создаем экземпляр объекта Workbook, вызвав его пустой конструктор
Workbook workbook = new Workbook("book1.xls");
 
  //Получение списка всех пользовательских свойств документа Excel file
DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
 
  //Доступ к пользовательскому свойству документа с помощью свойства index
DocumentProperty customProperty1 = customProperties[3];
 
  //Доступ к пользовательскому свойству документа с помощью свойства name
DocumentProperty customProperty2 = customProperties["Owner"];

[VB.NET]

'Создаем экземпляр объекта Workbook, вызвав его пустой конструктор
Dim workbook As Workbook = New Workbook("book1.xls")
 
'Получение списка всех пользовательских свойств документа Excel file
Dim customProperties As DocumentPropertyCollection = workbook.Worksheets.CustomDocumentProperties
 
'Доступ к пользовательскому свойству документа с помощью свойства index
Dim customProperty1 As DocumentProperty = customProperties(3)
 
'Доступ к пользовательскому свойству документа с помощью свойства name
Dim customProperty2 As DocumentProperty = customProperties("Owner")

```

### Смотрите также

* пространство имен [Aspose.Cells.Properties](../../aspose.cells.properties)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
