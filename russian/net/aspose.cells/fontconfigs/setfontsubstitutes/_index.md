---
title: "FontConfigs.SetFontSubstitutes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontConfigs. Имена заменяющих шрифтов для заданного оригинального названия шрифта"
type: docs
url: /ru/net/aspose.cells/fontconfigs/setfontsubstitutes/
---
## FontConfigs.SetFontSubstitutes method

Имена заменяющих шрифтов для заданного оригинального имени шрифта.

```csharp
public static void SetFontSubstitutes(string originalFontName, string[] substituteFontNames)
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

    public class FontConfigsMethodSetFontSubstitutesWithStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Оригинальное название шрифта, которое может быть недоступно
            string originalFontName = "Arial";
            
            // Имена заменяющих шрифтов, используемые когда оригинал недоступен
            string[] substituteFontNames = new string[] { "Liberation Sans", "Helvetica", "Verdana" };
            
            try
            {
                // Вызовите метод SetFontSubstitutes для настройки замен шрифтов
                FontConfigs.SetFontSubstitutes(originalFontName, substituteFontNames);
                
                Console.WriteLine($"Font substitutes set successfully for '{originalFontName}'");
                
                // Проверьте заменяющие шрифты, получив их
                string[] retrievedSubstitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("Current substitutes for '{0}':", originalFontName);
                foreach (string font in retrievedSubstitutes)
                {
                    Console.WriteLine("- " + font);
                }
                
                // Примените шрифт к ячейке для демонстрации замены
                worksheet.Cells["A1"].PutValue("Text with potential font substitution");
                Style style = worksheet.Cells["A1"].GetStyle();
                style.Font.Name = originalFontName;
                worksheet.Cells["A1"].SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFontSubstitutes method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("FontSubstitutionDemo.xlsx");
        }
    }
}
```

### См. также

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


