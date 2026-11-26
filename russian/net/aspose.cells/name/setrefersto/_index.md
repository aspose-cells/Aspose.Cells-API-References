---
title: "Name.SetRefersTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Name. Установить ссылку для этого Name"
type: docs
url: /ru/net/aspose.cells/name/setrefersto/
---
## Name.SetRefersTo method

Задать ссылку этого Name.

```csharp
public void SetRefersTo(string refersTo, bool isR1C1, bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| refersTo | String | Ссылка. |
| isR1C1 | Boolean | Является ли ссылка в формате R1C1. |
| isLocal | Boolean | Является ли ссылка отформатированной согласно локали. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodSetRefersToWithStringBooleanBooleanDemo
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

            try
            {
                // Вызвать SetRefersTo с параметрами (String, Boolean, Boolean)
                namedRange.SetRefersTo("=Sheet1!$A$1:$A$3", false, false);

                // Отобразить результат
                Console.WriteLine($"Named range 'MyNamedRange' now refers to: {namedRange.RefersTo}");

                // Проверить, используя именованный диапазон в формуле
                worksheet.Cells["B1"].Formula = "=SUM(MyNamedRange)";
                workbook.CalculateFormula();

                Console.WriteLine($"Result of SUM(MyNamedRange): {worksheet.Cells["B1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetRefersTo method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("NameMethodSetRefersToWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### См. также

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


