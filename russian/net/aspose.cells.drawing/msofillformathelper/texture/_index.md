---
title: "MsoFillFormatHelper.Texture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MsoFillFormatHelper. Получает тип текстурной заливки"
type: docs
url: /ru/net/aspose.cells.drawing/msofillformathelper/texture/
---
## MsoFillFormatHelper.Texture property

Получает тип текстурного заполнения.

```csharp
public TextureType Texture { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Reflection;

    public class MsoFillFormatHelperPropertyTextureDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте метку, чтобы пример имел смысл
            worksheet.Cells["A1"].Value = "Texture Property Demo";

            try
            {
                // Создайте экземпляр MsoFillFormatHelper с помощью рефлексии (нет публичного конструктора)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Отобразите текущее значение свойства Texture (только для чтения)
                Console.WriteLine($"Current Texture type: {fillHelper.Texture}");

                // Продемонстрируйте, что свойство только для чтения, попытавшись установить его (закомментировано)
                // fillHelper.Texture = TextureType.Canvas; // Это вызвало бы ошибку компиляции

                // Покажите все доступные типы текстур для справки
                Console.WriteLine("\nAvailable Texture Types:");
                foreach (TextureType textureType in Enum.GetValues(typeof(TextureType)))
                {
                    Console.WriteLine($"- {textureType}");
                }

                // Сохраните книгу, чтобы продемонстрировать успешное выполнение
                workbook.Save("TextureDemo.xlsx");

                Console.WriteLine("\nTexture property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during Texture demo: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [TextureType](../../texturetype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


