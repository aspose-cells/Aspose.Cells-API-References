---
title: "ContentTypePropertyCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ContentTypePropertyCollection. Добавляет информацию о свойствах типа контента"
type: docs
url: /ru/net/aspose.cells.properties/contenttypepropertycollection/add/
---
## Add(string, string) {#add}

Добавляет информацию о свойстве типа содержимого.

```csharp
public int Add(string name, string value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя свойства типа содержимого. |
| значение | String | Значение свойства типа содержимого. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            ContentTypePropertyCollection ctps = wb.ContentTypeProperties;
            ctps.Add("CustomProperty1", "SampleValue1");
            ctps.Add("CustomProperty2", "SampleValue2");
            
            wb.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_1}

Добавляет информацию о свойстве типа содержимого.

```csharp
public int Add(string name, string value, string type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя свойства типа содержимого. |
| значение | String | Значение свойства типа содержимого. |
| type | String | Тип свойства типа содержимого. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.ContentTypeProperties.Add("propertyName", "propertyValue", "string");
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


