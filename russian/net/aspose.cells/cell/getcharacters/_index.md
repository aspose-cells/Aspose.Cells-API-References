---
title: "Cell.GetCharacters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Возвращает все объекты Characters, представляющие диапазон символов в тексте ячейки."
type: docs
url: /ru/net/aspose.cells/cell/getcharacters/
---
## GetCharacters() {#getcharacters}

Возвращает все объекты Characters, представляющие диапазон символов в тексте ячейки.

```csharp
public FontSetting[] GetCharacters()
```

### Возвращаемое значение

Все объекты Characters

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите HTML‑форматированный текст в ячейку A1 с различными частями форматирования
            worksheet.Cells["A1"].HtmlString = "Normal text<div style=\"color: red;\">Red text</div>";

            // Получите информацию о форматировании символов из ячейки A1
            FontSetting[] fontSettings = worksheet.Cells["A1"].GetCharacters();

            // Выведите информацию о форматировании
            Console.WriteLine("Character formatting in cell A1:");
            for (int i = 0; i < fontSettings.Length; i++)
            {
                Console.WriteLine($"Part {i + 1}:");
                Console.WriteLine($"Start index: {fontSettings[i].StartIndex}");
                Console.WriteLine($"Length: {fontSettings[i].Length}");
                Console.WriteLine($"Font color: {fontSettings[i].Font.Color}");
                Console.WriteLine();
            }
        }
    }
}
```

### См. также

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCharacters(bool) {#getcharacters_1}

Возвращает все объекты Characters, представляющие диапазон символов в тексте ячейки.

```csharp
public FontSetting[] GetCharacters(bool flag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| флаг | Boolean | Указывает, применяется ли стиль таблицы к ячейке, если ячейка находится в таблице. |

### Возвращаемое значение

Все объекты Characters

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersWithBooleanDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте текст в ячейку C8 с форматированием
            Cell cell = worksheet.Cells["C8"];
            cell.PutValue("Formatted Text");
            
            // Форматировать части текста
            FontSetting fs1 = cell.Characters(0, 8);
            fs1.Font.Color = System.Drawing.Color.White;
            
            FontSetting fs2 = cell.Characters(9, 4);
            fs2.Font.Color = System.Drawing.Color.Blue;
            
            // Получить все настройки шрифта с форматированием
            FontSetting[] fontSettings = cell.GetCharacters(true);
            
            // Отобразить цвета шрифта
            Console.WriteLine("Font colors in cell C8:");
            foreach (FontSetting fs in fontSettings)
            {
                Console.WriteLine(fs.Font.Color);
            }
        }
    }
}
```

### См. также

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


