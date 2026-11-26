---
title: "SmartTagCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SmartTagCollection. Добавляет умный тег"
type: docs
url: /ru/net/aspose.cells.markup/smarttagcollection/add/
---
## SmartTagCollection.Add method

Добавляет смарт‑тег.

```csharp
public int Add(string uri, string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| uri | String | Указывает URI пространства имён умного тега |
| name | String | Указывает имя умного тега. |

### Возвращаемое значение

Индекс смарт‑тега в списке.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Added smart tag at index: " + tagIndex);
            workbook.Save("SmartTagCollectionAddExample.xlsx");
        }
    }
}
```

### См. также

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


