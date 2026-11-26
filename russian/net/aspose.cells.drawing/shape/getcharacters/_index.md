---
title: "Shape.GetCharacters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Возвращает все объекты Characters, представляющие диапазон символов в тексте"
type: docs
url: /ru/net/aspose.cells.drawing/shape/getcharacters/
---
## Shape.GetCharacters method

Возвращает все объекты Characters, представляющие диапазон символов внутри текста.

```csharp
[Obsolete("Use Shape.GetRichFormattings() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetCharacters()
```

### Возвращаемое значение

Все объекты Characters

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Shape.GetRichFormattings(). Этот метод будет удалён через 12 месяцев, начиная с ноября 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте форму текстового поля в лист с указанием всех необходимых параметров
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample Text";

            // Получите символы из формы
            ArrayList characters = shape.GetCharacters();

            // Отобразите информацию о каждом символе
            foreach (FontSetting charSetting in characters)
            {
                Console.WriteLine($"Font: {charSetting.Font.Name}, Size: {charSetting.Font.Size}");
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


