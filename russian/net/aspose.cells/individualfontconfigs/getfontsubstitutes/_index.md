---
title: "IndividualFontConfigs.GetFontSubstitutes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IndividualFontConfigs. Возвращает массив, содержащий имена замен шрифтов, которые будут использоваться, если оригинальный шрифт не представлен"
type: docs
url: /ru/net/aspose.cells/individualfontconfigs/getfontsubstitutes/
---
## IndividualFontConfigs.GetFontSubstitutes method

Возвращает массив, содержащий имена заменяющих шрифтов, которые будут использоваться, если оригинальный шрифт не представлен.

```csharp
public string[] GetFontSubstitutes(string originalFontName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| originalFontName | String | originalFontName |

### Возвращаемое значение

Массив, содержащий имена заменяющих шрифтов, которые будут использоваться, если оригинальный шрифт не представлен.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Создать индивидуальные конфигурации шрифтов
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Установить замену шрифтов для "Arial"
            fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Calibri" });

            try
            {
                // Получить замену шрифтов для "Arial"
                string[] substitutes = fontConfigs.GetFontSubstitutes("Arial");

                Console.WriteLine("Font substitutes for Arial:");
                foreach (string font in substitutes)
                {
                    Console.WriteLine(font);
                }

                // Создать книгу для демонстрации эффекта
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Установить стиль с оригинальным шрифтом
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "This text uses Arial font which may be substituted";

                // Сохраните книгу
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSubstitutes method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


