---
title: "SmartTagPropertyCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SmartTagPropertyCollection. Получает объект SmartTagProperty"
type: docs
url: /ru/net/aspose.cells.markup/smarttagpropertycollection/item/
---
## SmartTagPropertyCollection indexer (1 of 2)

Получает объект [`SmartTagProperty`](../../smarttagproperty/).

```csharp
public SmartTagProperty this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс |

### Возвращаемое значение

Возвращает объект [`SmartTagProperty`](../../smarttagproperty/) объект.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать коллекцию свойств смарт-тега
            SmartTagPropertyCollection properties = new SmartTagPropertyCollection();

            // Добавьте свойства в коллекцию
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Доступ к свойствам с помощью индексатора Item
            SmartTagProperty property1 = properties[index1];
            SmartTagProperty property2 = properties[index2];

            // Отобразить текущие значения свойств
            Console.WriteLine("Property1 Name: " + property1.Name);
            Console.WriteLine("Property1 Value: " + property1.Value);
            Console.WriteLine("Property2 Name: " + property2.Name);
            Console.WriteLine("Property2 Value: " + property2.Value);

            // Примечание: свойство Item только для чтения, поэтому мы не можем напрямую присвоить ему значение
            // Вместо этого мы можем изменить свойства возвращённых объектов SmartTagProperty
            property1.Value = "UpdatedValue1";
            property2.Value = "UpdatedValue2";

            // Отобразить обновленные значения
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property1 Value: " + properties[index1].Value);
            Console.WriteLine("Property2 Value: " + properties[index2].Value);

            // Сохранить книгу (хотя смарт-теги явно не сохраняются при простом сохранении)
            workbook.Save("SmartTagPropertyDemo.xlsx");
        }
    }
}
```

### См. также

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagPropertyCollection indexer (2 of 2)

Получает объект [`SmartTagProperty`](../../smarttagproperty/) по имени свойства.

```csharp
public SmartTagProperty this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя свойства. |

### Возвращаемое значение

Возвращает объект [`SmartTagProperty`](../../smarttagproperty/) объект.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создать настройку смарт-тега и добавить смарт-тег
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
                int smartTagIndex = smartTagSetting.Add(0, 0);
                SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
                smartTags.Add("http://example.com", "example");

                // Получить смарт-тег и его свойства
                SmartTag smartTag = smartTags[0];
                SmartTagPropertyCollection properties = smartTag.Properties;

                // Добавить несколько свойств для демонстрации свойства Item
                properties.Add("Author", "John Doe");
                properties.Add("Version", "1.0");

                // Доступ к свойствам с помощью индексатора Item (по индексу)
                SmartTagProperty firstProperty = properties[0];
                SmartTagProperty secondProperty = properties[1];

                // Отобразите значения свойств
                Console.WriteLine("First Property Name: " + firstProperty.Name);
                Console.WriteLine("First Property Value: " + firstProperty.Value);
                Console.WriteLine("Second Property Name: " + secondProperty.Name);
                Console.WriteLine("Second Property Value: " + secondProperty.Value);

                // Сохраните книгу
                workbook.Save("SmartTagItemDemo.xlsx");
                Console.WriteLine("SmartTagItemDemo.xlsx created successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


