---
title: "XmlDataBinding.Url"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlDataBinding. Получает исходный URL этой привязки данных"
type: docs
url: /ru/net/aspose.cells/xmldatabinding/url/
---
## XmlDataBinding.Url property

Получает URL источника этой привязки данных.

```csharp
public string Url { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class XmlDataBindingPropertyUrlDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте два листа
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");

            // Добавьте объекты списка и XML‑карты
            ListObject list1 = workbook.Worksheets[0].ListObjects[0];
            ListObject list2 = workbook.Worksheets[1].ListObjects[0];
            
            // Получить URL привязки XML‑данных (Url доступен только для чтения)
            string url1 = list1.XmlMap.DataBinding.Url;
            string url2 = list2.XmlMap.DataBinding.Url;

            // Отобразить URL‑ы
            Console.WriteLine("Sheet1 ListObject XML URL: " + url1);
            Console.WriteLine("Sheet2 ListObject XML URL: " + url2);

            // Сохраните книгу
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### См. также

* class [XmlDataBinding](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


