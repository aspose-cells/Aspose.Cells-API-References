---
title: "SmartTagSetting.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SmartTagSetting. Добавляет объект SmartTagCollection в ячейку"
type: docs
url: /ru/net/aspose.cells.markup/smarttagsetting/add/
---
## Add(int, int) {#add}

Добавляет объект [`SmartTagCollection`](../../smarttagcollection/) в ячейку.

```csharp
public int Add(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Строка ячейки. |
| column | Int32 | Столбец ячейки. |

### Возвращаемое значение

Возвращает индекс объекта [`SmartTagCollection`](../../smarttagcollection/) в листе.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Add to cell A1 (row 0, column 0)

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart Tags Count: " + smartTagSetting.Count.ToString());
            workbook.Save("SmartTagDemo.xlsx");
        }
    }
}
```

### См. также

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Добавить смарт‑теги ячейки.

```csharp
public int Add(string cellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить экземпляр SmartTagSetting
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            
            try
            {
                // Вызвать метод Add с параметром String
                int index = smartTagSetting.Add("A1");
                
                Console.WriteLine($"SmartTag added successfully at index: {index}");
                
                // Добавьте некоторый контент, чтобы продемонстрировать эффект
                worksheet.Cells["A1"].PutValue("This cell has a smart tag");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("SmartTagSettingMethodAddWithStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


