---
title: "NameCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод NameCollection. Определяет новое имя"
type: docs
url: /ru/net/aspose.cells/namecollection/add/
---
## NameCollection.Add method

Определяет новое имя.

```csharp
public int Add(string text)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | String | Текст, используемый в качестве имени. |

### Возвращаемое значение

[`Name`](../../name/) object index.

### Примечания

Имя не может содержать пробелы и не должно выглядеть как ссылки на ячейки.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = wb.Worksheets[0];
            
            // Добавьте имя со строковой ссылкой
            int index = wb.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = wb.Worksheets.Names[index];
            
            // Установите формулу, на которую ссылается имя
            namedRange.RefersTo = "=Sheet1!$A$1:$B$10";
            
            // Проверьте и выведите результаты
            Console.WriteLine("Named Range RefersTo: " + namedRange.RefersTo);
            Console.WriteLine("Named Range Index: " + index);
            
            // Получите диапазон и отобразите его адрес
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Range Address: " + range.Address);
        }
    }
}
```

### См. также

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


