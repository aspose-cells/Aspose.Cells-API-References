---
title: "HyperlinkCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод HyperlinkCollection. Добавляет гиперссылку в указанную ячейку или диапазон ячеек."
type: docs
url: /ru/net/aspose.cells/hyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Добавляет гиперссылку в указанную ячейку или диапазон ячеек.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Первая строка диапазона гиперссылки. |
| firstColumn | Int32 | Первый столбец диапазона гиперссылки. |
| totalRows | Int32 | Количество строк в этом диапазоне гиперссылки. |
| totalColumns | Int32 | Количество столбцов этого диапазона гиперссылки. |
| address | String | Адрес гиперссылки. |

### Возвращаемое значение

[`Hyperlink`](../../hyperlink/) object index.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить гиперссылку, используя координаты строки/столбца и размеры
            worksheet.Hyperlinks.Add(0, 0, 1, 1, "http://www.aspose.com");
            worksheet.Hyperlinks.Add(1, 0, 1, 1, "c:\\book1.xls");
            
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### См. также

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_1}

Добавляет гиперссылку в указанную ячейку или диапазон ячеек.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |
| totalRows | Int32 | Количество строк в этом диапазоне гиперссылки. |
| totalColumns | Int32 | Количество столбцов этого диапазона гиперссылки. |
| address | String | Адрес гиперссылки. |

### Возвращаемое значение

[`Hyperlink`](../../hyperlink/) object index.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Добавить гиперссылку в ячейку A1 с адресом "www.aspose.com"
            hyperlinks.Add("A1", 1, 1, "www.aspose.com");
            
            // Отобразить адрес гиперссылки
            Console.WriteLine("Hyperlink Address: " + worksheet.Cells["A1"].StringValue);
            
            // Изменить отображаемый текст
            worksheet.Cells["A1"].PutValue("Click Here");
            Console.WriteLine("Display Text: " + hyperlinks[0].TextToDisplay);
            
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### См. также

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, string, string) {#add_2}

Добавляет гиперссылку в указанную ячейку или диапазон ячеек.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| startCellName | String | Ячейка в левом верхнем углу диапазона. |
| endCellName | String | Ячейка в правом нижнем углу диапазона. |
| address | String | Адрес гиперссылки. |
| textToDisplay | String | Текст, который будет отображаться для указанной гиперссылки. |
| screenTip | String | Текст screenTip для указанной гиперссылки. |

### Возвращаемое значение

[`Hyperlink`](../../hyperlink/) object index.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Продемонстрировать метод Add с параметрами (String, String, String, String, String)
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            workbook.Save("HyperlinkCollectionExample.xlsx");
        }
    }
}
```

### См. также

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


