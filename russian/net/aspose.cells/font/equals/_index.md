---
title: "Font.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Font. Проверяет, равны ли два шрифта"
type: docs
url: /ru/net/aspose.cells/font/equals/
---
## Font.Equals method

Проверяет, равны ли два шрифта.

```csharp
public bool Equals(Font font)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| шрифт | Шрифт | Сравненный объект шрифта. |

### Возвращаемое значение

Истина, если равен сравниваемому объекту шрифта.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontMethodEqualsWithFontDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте два объекта шрифта для сравнения
            Font font1 = workbook.CreateStyle().Font;
            font1.Name = "Arial";
            font1.Size = 12;
            font1.IsBold = true;
            font1.Color = System.Drawing.Color.Black;

            Font font2 = workbook.CreateStyle().Font;
            font2.Name = "Arial";
            font2.Size = 12;
            font2.IsBold = true;
            font2.Color = System.Drawing.Color.Black;

            try
            {
                // Вызовите метод Equals для сравнения шрифтов
                bool areEqual = font1.Equals(font2);

                // Отобразить результат
                Console.WriteLine($"The fonts are equal: {areEqual}");

                // Измените один шрифт, чтобы они стали разными
                font2.IsItalic = true;
                areEqual = font1.Equals(font2);
                Console.WriteLine($"After modification, the fonts are equal: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("FontEqualsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


