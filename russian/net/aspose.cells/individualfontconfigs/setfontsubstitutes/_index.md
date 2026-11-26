---
title: "IndividualFontConfigs.SetFontSubstitutes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод IndividualFontConfigs. Устанавливает имена замен шрифтов для заданного оригинального имени шрифта"
type: docs
url: /ru/net/aspose.cells/individualfontconfigs/setfontsubstitutes/
---
## IndividualFontConfigs.SetFontSubstitutes method

Устанавливает имена заменяющих шрифтов для заданного оригинального имени шрифта.

```csharp
public void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| originalFontName | String | Оригинальное название шрифта. |
| substituteFontNames | String[] | Список имен заменяющих шрифтов, используемых если оригинальный шрифт не представлен. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // Создать экземпляр IndividualFontConfigs
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Оригинальное имя шрифта и его заменители
            string originalFont = "Arial";
            string[] substitutes = new string[] { "Helvetica", "Verdana", "Times New Roman" };

            try
            {
                // Вызвать SetFontSubstitutes с указанными параметрами
                fontConfigs.SetFontSubstitutes(originalFont, substitutes);

                Console.WriteLine($"Successfully set font substitutes for '{originalFont}'");
                Console.WriteLine("Substitutes are:");
                foreach (var sub in substitutes)
                {
                    Console.WriteLine($"- {sub}");
                }

                // Создать книгу для демонстрации эффекта
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Установить стиль с оригинальным шрифтом
                Style style = workbook.CreateStyle();
                style.Font.Name = originalFont;
                style.Font.Size = 14;
                
                worksheet.Cells["A1"].Value = "This text uses " + originalFont;
                worksheet.Cells["A1"].SetStyle(style);

                // Сохраните книгу
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting font substitutes: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


