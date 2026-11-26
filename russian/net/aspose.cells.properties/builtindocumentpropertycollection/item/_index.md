---
title: "BuiltInDocumentPropertyCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BuiltInDocumentPropertyCollection. Возвращает объект DocumentProperty по имени свойства"
type: docs
url: /ru/net/aspose.cells.properties/builtindocumentpropertycollection/item/
---
## BuiltInDocumentPropertyCollection indexer

Возвращает объект [`DocumentProperty`](../../documentproperty/) по имени свойства.

```csharp
public override DocumentProperty this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя свойства без учёта регистра для получения. |

### Примечания

Строковые имена свойств соответствуют именам типизированных свойств, доступных из [`BuiltInDocumentPropertyCollection`](../).

Если вы запрашиваете свойство, которого нет в документе, но имя свойства распознаётся как допустимое встроенное имя, создаётся новое [`DocumentProperty`](../../documentproperty/), добавляется в коллекцию и возвращается. Новому свойству присваивается значение по умолчанию (пустая строка, ноль, false или DateTime.MinValue в зависимости от типа встроенного свойства).

Если вы запрашиваете свойство, которого нет в документе, и имя не распознаётся как встроенное, возвращается null.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установите встроенное свойство документа, используя соответствующий метод
            workbook.BuiltInDocumentProperties["Version"].Value = "15.0300";
            
            // Получите доступ и выведите значение свойства
            Console.WriteLine("Version: " + workbook.BuiltInDocumentProperties["Version"].Value);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Загрузите сохранённую книгу и проверьте свойство
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Version: " + loadedWorkbook.BuiltInDocumentProperties["Version"].Value);
        }
    }
}
```

### См. также

* class [DocumentProperty](../../documentproperty/)
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


