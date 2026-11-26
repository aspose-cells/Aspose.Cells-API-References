---
title: "Класс ContentTypeProperty"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Properties.ContentTypeProperty. Представляет информацию об идентификаторе"
type: docs
url: /ru/net/aspose.cells.properties/contenttypeproperty/
---
## ContentTypeProperty class

Представляет информацию об идентификаторе.

```csharp
public class ContentTypeProperty
```

## Свойства

| Имя | Описание |
| --- | --- |
| [IsNillable](../../aspose.cells.properties/contenttypeproperty/isnillable/) { get; set; } | Указывает, может ли значение быть пустым. |
| [Name](../../aspose.cells.properties/contenttypeproperty/name/) { get; set; } | Возвращает или задает имя объекта. |
| [Type](../../aspose.cells.properties/contenttypeproperty/type/) { get; set; } | Получает и задаёт тип свойства. |
| [Value](../../aspose.cells.properties/contenttypeproperty/value/) { get; set; } | Возвращает или задает значение свойства типа содержимого. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class ContentTypePropertyDemo
    {
        public static void ContentTypePropertyExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Добавить новое свойство типа содержимого
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");

            // Получить доступ к только что добавленному свойству
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Установка свойств
            property.Name = "Admin";
            property.Value = "Aspose";
            property.Type = "text";
            property.IsNillable = true;

            // Сохраните файл Excel
            workbook.Save("ContentTypePropertyExample.xlsx");
            workbook.Save("ContentTypePropertyExample.pdf");
            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


