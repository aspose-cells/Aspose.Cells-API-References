---
title: "FontConfigs.GetFontSubstitutes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FontConfigs. Возвращает массив, содержащий имена заменяющих шрифтов, которые будут использоваться, если оригинальный шрифт отсутствует"
type: docs
url: /ru/net/aspose.cells/fontconfigs/getfontsubstitutes/
---
## FontConfigs.GetFontSubstitutes method

Возвращает массив, содержащий имена заменяющих шрифтов, которые будут использоваться, если оригинальный шрифт отсутствует.

```csharp
public static string[] GetFontSubstitutes(string originalFontName)
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

    public class FontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Инициализировать FontConfigs
            FontConfigs fontConfigs = new FontConfigs();

            try
            {
                // Вызвать GetFontSubstitutes с именем шрифта
                string originalFontName = "Arial";
                string[] substitutes = FontConfigs.GetFontSubstitutes(originalFontName);

                // Отобразите результаты
                Console.WriteLine($"Substitute fonts for '{originalFontName}':");
                if (substitutes != null && substitutes.Length > 0)
                {
                    foreach (string substitute in substitutes)
                    {
                        Console.WriteLine(substitute);
                    }
                }
                else
                {
                    Console.WriteLine("No substitutes found for the specified font.");
                }

                // Продемонстрировать установку замен и их получение
                string[] newSubstitutes = new string[] { "Liberation Sans", "DejaVu Sans" };
                FontConfigs.SetFontSubstitutes(originalFontName, newSubstitutes);

                // Получить заменяющие шрифты снова для проверки
                substitutes = FontConfigs.GetFontSubstitutes(originalFontName);
                Console.WriteLine("\nAfter setting substitutes:");
                foreach (string substitute in substitutes)
                {
                    Console.WriteLine(substitute);
                }
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

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


