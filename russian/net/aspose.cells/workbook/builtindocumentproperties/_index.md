---
title: "Workbook.BuiltInDocumentProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Возвращает коллекцию DocumentProperty, представляющую все встроенные свойства документа электронной таблицы"
type: docs
url: /ru/net/aspose.cells/workbook/builtindocumentproperties/
---
## Workbook.BuiltInDocumentProperties property

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
    public class WorkbookPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получайте доступ и изменяйте встроенные свойства документа
            DocumentProperty authorProperty = workbook.BuiltInDocumentProperties["Author"];
            authorProperty.Value = "John Smith";
            
            DocumentProperty titleProperty = workbook.BuiltInDocumentProperties["Title"];
            titleProperty.Value = "Sample Workbook";
            
            // Отобразите изменённые свойства
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Title: " + workbook.BuiltInDocumentProperties["Title"].Value);
        }
    }
}
```

### См. также

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


