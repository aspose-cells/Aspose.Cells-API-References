---
title: "ContentTypePropertyCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ContentTypePropertyCollection. Получает свойство типа содержимого по указанному индексу"
type: docs
url: /ru/net/aspose.cells.properties/contenttypepropertycollection/item/
---
## ContentTypePropertyCollection indexer (1 of 2)

Получает свойство типа содержимого по указанному индексу.

```csharp
public ContentTypeProperty this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

Свойство типа содержимого

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Добавьте свойства типа содержимого и продемонстрируйте использование свойства Item
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Доступ к свойствам с помощью индексатора Item
            Console.WriteLine($"Property1 IsNillable: {workbook.ContentTypeProperties[0].IsNillable}");
            Console.WriteLine($"Property2 IsNillable: {workbook.ContentTypeProperties[1].IsNillable}");
            
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### См. также

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## ContentTypePropertyCollection indexer (2 of 2)

Получает свойство типа содержимого по имени свойства.

```csharp
public ContentTypeProperty this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя свойства. |

### Возвращаемое значение

Свойство типа содержимого

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Добавить свойство типа содержимого
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Доступ к свойству с помощью индексатора Item
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Изменить значения свойств
            property.Value = "UpdatedValue";
            property.IsNillable = false;
            
            // Сохранить книгу
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### См. также

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


