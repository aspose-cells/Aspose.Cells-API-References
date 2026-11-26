---
title: "Name.GetRefersTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Name. Получить ссылку на этот Name"
type: docs
url: /ru/net/aspose.cells/name/getrefersto/
---
## GetRefersTo(bool, bool) {#getrefersto}

Получить ссылку этого Name.

```csharp
public string GetRefersTo(bool isR1C1, bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | Boolean | Нужно ли форматировать ссылку как R1C1. |
| isLocal | Boolean | Нужно ли форматировать ссылку в соответствии с локалью. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodGetRefersToWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные в ячейки
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Создать именованный диапазон
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";

            try
            {
                // Вызвать GetRefersTo с форматом R1C1 и локальной областью
                string refersToR1C1Local = namedRange.GetRefersTo(true, true);
                Console.WriteLine("R1C1 format with local scope: " + refersToR1C1Local);

                // Вызвать GetRefersTo с форматом A1 и глобальной областью
                string refersToA1Global = namedRange.GetRefersTo(false, false);
                Console.WriteLine("A1 format with global scope: " + refersToA1Global);

                // Показать детали именованного диапазона
                Console.WriteLine("Named range text: " + namedRange.Text);
                Console.WriteLine("Full text: " + namedRange.FullText);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("NameMethodGetRefersToDemo.xlsx");
        }
    }
}
```

### См. также

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRefersTo(bool, bool, int, int) {#getrefersto_1}

Получить ссылку этого Name на основе указанной ячейки.

```csharp
public string GetRefersTo(bool isR1C1, bool isLocal, int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | Boolean | Нужно ли форматировать ссылку как R1C1. |
| isLocal | Boolean | Нужно ли форматировать ссылку в соответствии с локалью. |
| строка | Int32 | Индекс строки ячейки. |
| column | Int32 | Индекс столбца ячейки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные в ячейки
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Создать именованный диапазон
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";

            try
            {
                // Вызвать GetRefersTo с конкретными параметрами (isR1C1, isLocal, row, column)
                string refersTo = namedRange.GetRefersTo(false, false, 0, 0);
                
                Console.WriteLine("Named range refers to: " + refersTo);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean, Int32, Int32)");

                // Изменить именованный диапазон на основе результата
                if (!string.IsNullOrEmpty(refersTo))
                {
                    worksheet.Cells["B1"].PutValue("Named Range Refers To:");
                    worksheet.Cells["B2"].PutValue(refersTo);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo.xlsx");
        }
    }
}
```

### См. также

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


