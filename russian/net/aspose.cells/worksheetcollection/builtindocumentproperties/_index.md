---
title: "WorksheetCollection.BuiltInDocumentProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Возвращает коллекцию DocumentProperty, представляющую все встроенные свойства документа электронной таблицы"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/builtindocumentproperties/
---
## WorksheetCollection.BuiltInDocumentProperties property

Возвращает коллекцию [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/), представляющую все встроенные свойства документа электронной таблицы.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Примечания

Новое свойство нельзя добавить в список встроенных свойств документа. Можно только получить встроенное свойство и изменить его значение. Ниже приведён список имён встроенных свойств:

Заголовок

Тема

Автор

Ключевые слова

Комментарии

Шаблон

Последний автор

Номер ревизии

Название приложения

Дата последней печати

Дата создания

Время последнего сохранения

Общее время редактирования

Количество страниц

Количество слов

Количество символов

Безопасность

Категория

Формат

Менеджер

Компания

Количество байт

Количество строк

Количество абзацев

Количество слайдов

Количество заметок

Количество скрытых слайдов

Количество мультимедийных клипов

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            DocumentProperty authorProperty = workbook.Worksheets.BuiltInDocumentProperties["Author"];
            authorProperty.Value = "John Smith";
            
            DocumentProperty titleProperty = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            titleProperty.Value = "Sample Document";
            
            Console.WriteLine("Document properties set successfully");
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


