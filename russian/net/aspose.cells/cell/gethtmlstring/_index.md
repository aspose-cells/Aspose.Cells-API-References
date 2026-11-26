---
title: "Cell.GetHtmlString"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получает HTML-строку, содержащую данные и некоторые форматы в этой ячейке"
type: docs
url: /ru/net/aspose.cells/cell/gethtmlstring/
---
## Cell.GetHtmlString method

Получает HTML-строку, содержащую данные и некоторые форматы в этой ячейке.

```csharp
public string GetHtmlString(bool html5)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| html5 | Boolean | Указывает, совместимо ли значение с html5 |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetHtmlStringWithBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите примерное значение ячейки с форматированием
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            style.Font.Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            // Продемонстрируйте GetHtmlString с булевым параметром
            string htmlWithoutDiv = cell.GetHtmlString(false);
            string htmlWithDiv = cell.GetHtmlString(true);
            
            Console.WriteLine("HTML without div wrapper:");
            Console.WriteLine(htmlWithoutDiv);
            Console.WriteLine("\nHTML with div wrapper:");
            Console.WriteLine(htmlWithDiv);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


