---
title: "WebExtensionPropertyCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionPropertyCollection. Получает свойство веб-расширения по индексу"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionpropertycollection/item/
---
## WebExtensionPropertyCollection indexer (1 of 2)

Получает свойство веб-расширения по индексу.

```csharp
public WebExtensionProperty this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

Свойство веб-расширения.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать коллекцию свойств веб-расширения
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Добавьте некоторые свойства
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Доступ к свойствам с помощью индексатора Item
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Измените значения свойств через коллекцию
            properties[index1].Value = "UpdatedValue1";
            properties[index2].Value = "UpdatedValue2";

            // Продемонстрируйте изменения
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Сохраните книгу (хотя свойства веб‑расширения не будут видны в сохранённом файле без надлежащей настройки)
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### См. также

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)

---

## WebExtensionPropertyCollection indexer (2 of 2)

Получает свойство веб‑расширения.

```csharp
public WebExtensionProperty this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя свойства. |

### Возвращаемое значение

Свойство веб-расширения.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать коллекцию свойств веб-расширения
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Добавьте свойства в коллекцию
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");

            // Получайте свойства с помощью индексатора Item
            WebExtensionProperty property1 = properties["Property1"];
            Console.WriteLine("Property1 value: " + property1.Value);

            WebExtensionProperty property2 = properties["Property2"];
            Console.WriteLine("Property2 value: " + property2.Value);

            // Измените значения свойств (примечание: Item только для чтения, поэтому необходимо использовать Add/Remove)
            properties.RemoveAt("Property1");
            properties.Add("Property1", "NewValue1");

            // Показать обновлённое значение
            property1 = properties["Property1"];
            Console.WriteLine("Updated Property1 value: " + property1.Value);

            // Сохраните книгу
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### См. также

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


