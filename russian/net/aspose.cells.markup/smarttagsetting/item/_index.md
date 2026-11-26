---
title: "SmartTagSetting.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SmartTagSetting. Получает объект SmartTagCollection по индексу"
type: docs
url: /ru/net/aspose.cells.markup/smarttagsetting/item/
---
## SmartTagSetting indexer (1 of 3)

Получает объект [`SmartTagCollection`](../../smarttagcollection/) по индексу.

```csharp
public SmartTagCollection this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| index | Индекс объекта [`SmartTagCollection`](../../smarttagcollection/) в списке. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            
            // Продемонстрировать использование свойства Item
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
            smartTags.Add("http://docs.aspose.com", "docs");
            
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Version", "1.0");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### См. также

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (2 of 3)

Получает объект [`SmartTagCollection`](../../smarttagcollection/) ячейки.

```csharp
public SmartTagCollection this[int row, int column] { get; }
```

| Параметр | Описание |
| --- | --- |
| строка | Индекс строки ячейки. |
| column | Индекс столбца ячейки |

### Возвращаемое значение

Возвращает объект [`SmartTagCollection`](../../smarttagcollection/) ячейки. Возвращает null, если в ячейке нет умных тегов.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            // Продемонстрировать использование свойства Item
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart tags in cell A1: " + smartTagCollection.Count);
            Console.WriteLine("Namespace URI: " + smartTagCollection[0].Uri);
            Console.WriteLine("Tag name: " + smartTagCollection[0].Name);

            workbook.Save("SmartTagDemo.xlsx");
        }
    }
}
```

### См. также

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (3 of 3)

Получает объект [`SmartTagCollection`](../../smarttagcollection/) ячейки.

```csharp
public SmartTagCollection this[string cellName] { get; }
```

| Параметр | Описание |
| --- | --- |
| cellName | Имя ячейки. |

### Возвращаемое значение

Возвращает объект [`SmartTagCollection`](../../smarttagcollection/) ячейки. Возвращает null, если в ячейке нет умных тегов.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingPropertyItemDemo2
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Получить доступ к SmartTagSetting листа
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;

                // Добавить умный тег в ячейку A1 (строка 0, столбец 0)
                int smartTagIndex = smartTagSetting.Add(0, 0);

                // Продемонстрировать использование свойства Item (индексатор)
                SmartTagCollection smartTagCollection = smartTagSetting[smartTagIndex];

                // Добавить смарт‑тег в коллекцию
                smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

                // Отобразить информацию об умном теге
                Console.WriteLine("Number of smart tags in collection: " + smartTagCollection.Count);
                if (smartTagCollection.Count > 0)
                {
                    Console.WriteLine("First smart tag URI: " + smartTagCollection[0].Uri);
                    Console.WriteLine("First smart tag name: " + smartTagCollection[0].Name);
                }

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

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


