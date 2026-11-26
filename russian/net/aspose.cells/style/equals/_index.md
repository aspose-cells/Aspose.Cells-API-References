---
title: "Style.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Style. Определяет, равны ли два экземпляра Style"
type: docs
url: /ru/net/aspose.cells/style/equals/
---
## Style.Equals method

Определяет, равны ли два экземпляра Style.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object | Объект Style для сравнения с текущим объектом Style. |

### Возвращаемое значение

true, если указанный объект равен текущему объекту; иначе false.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте два стиля для сравнения
            Style style1 = workbook.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.HorizontalAlignment = TextAlignmentType.Center;

            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Arial";
            style2.Font.Size = 12;
            style2.HorizontalAlignment = TextAlignmentType.Center;

            try
            {
                // Вызовите метод Equals для сравнения стилей
                bool areEqual = style1.Equals((object)style2);

                // Отобразить результат
                Console.WriteLine($"The styles are equal: {areEqual}");

                // Примените стили, чтобы продемонстрировать их идентичность
                if (areEqual)
                {
                    Cell cell1 = worksheet.Cells["A1"];
                    cell1.PutValue("Style 1");
                    cell1.SetStyle(style1);

                    Cell cell2 = worksheet.Cells["A2"];
                    cell2.PutValue("Style 2");
                    cell2.SetStyle(style2);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("StyleEqualsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


