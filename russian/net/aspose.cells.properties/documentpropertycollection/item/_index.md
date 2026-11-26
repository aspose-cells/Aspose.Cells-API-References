---
title: "DocumentPropertyCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DocumentPropertyCollection. Возвращает объект DocumentProperty по имени свойства"
type: docs
url: /ru/net/aspose.cells.properties/documentpropertycollection/item/
---
## DocumentPropertyCollection indexer (1 of 2)

Возвращает объект [`DocumentProperty`](../../documentproperty/) по имени свойства.

```csharp
public virtual DocumentProperty this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя свойства без учёта регистра для получения. |

### Примечания

Возвращает null, если свойство с указанным именем не найдено.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            string key = "TemplateGUID";
            object value = "TestValue123";

            if (wb.Worksheets.CustomDocumentProperties.Contains(key))
            {
                wb.Worksheets.CustomDocumentProperties[key].Value = value;
            }
            else
            {
                wb.Worksheets.CustomDocumentProperties.Add(key, value.ToString());
            }

            // Проверьте, что значение было установлено с помощью свойства Item
            Console.WriteLine("Property Value: " + wb.Worksheets.CustomDocumentProperties[key].Value);
        }
    }
}
```

### См. также

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## DocumentPropertyCollection indexer (2 of 2)

Возвращает объект [`DocumentProperty`](../../documentproperty/) по индексу.

```csharp
public DocumentProperty this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| index | Индекс (нумерация с нуля) [`DocumentProperty`](../../documentproperty/) для получения. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить встроенные свойства документа
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Установить встроенные свойства (не добавлять)
            properties.Author = "John Doe";
            properties.Company = "Aspose";
            properties["Version"].Value = "1.0";

            // Доступ к свойствам с помощью индексатора Item
            Console.WriteLine("Property 0: " + properties[0].Name + " = " + properties[0].Value);
            Console.WriteLine("Property 1: " + properties[1].Name + " = " + properties[1].Value);
            Console.WriteLine("Property 2: " + properties[2].Name + " = " + properties[2].Value);

            // Получайте доступ к свойству по имени
            DocumentProperty authorProp = properties["Author"];
            Console.WriteLine("Author property: " + authorProp.Value);

            // Изменить свойство
            properties["Version"].Value = "2.0";
            Console.WriteLine("Updated Version: " + properties["Version"].Value);
        }
    }
}
```

### См. также

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


