---
title: "HtmlSaveOptions.EnableCssCustomProperties"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Оптимизирует вывод html с помощью пользовательских CSS‑свойств. Например, в сценарии, когда один base64‑изображение используется несколько раз с пользовательским свойством, данные изображения нужно сохранить только один раз, что повышает производительность получаемого html. Значение по умолчанию — false."
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/enablecsscustomproperties/
---
## HtmlSaveOptions.EnableCssCustomProperties property

Оптимизировать вывод HTML с помощью пользовательских свойств CSS. Например, если один base64‑изображение используется несколько раз, с пользовательским свойством данные изображения сохраняются один раз, что повышает производительность получаемого HTML. Значение по умолчанию — false.

```csharp
public bool EnableCssCustomProperties { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class HtmlSaveOptionsPropertyEnableCssCustomPropertiesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные с форматированием
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;

            // Добавьте изображение, которое будет повторяться в нескольких ячейках
            int imgIndex = worksheet.Pictures.Add(1, 1, "logo.png");
            Picture pic = worksheet.Pictures[imgIndex];
            pic.Move(1, 1); // Using Move instead of LeftOffset/TopOffset
            pic.Width = 100;
            pic.Height = 100;

            // Скопируйте изображение в другое место
            worksheet.Cells["D5"].PutValue("Same image reference:");
            int imgIndex2 = worksheet.Pictures.Add(5, 3, "logo.png");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            pic2.Move(5, 3); // Using Move instead of LeftOffset/TopOffset
            pic2.Width = 100;
            pic2.Height = 100;

            // Создать экземпляр HtmlSaveOptions
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions();

            // Отобразите текущее значение
            Console.WriteLine("Current EnableCssCustomProperties value: " + htmlOptions.EnableCssCustomProperties);

            // Установите в true, чтобы оптимизировать вывод CSS
            htmlOptions.EnableCssCustomProperties = true;

            // Сохранить с оптимизацией CSS
            workbook.Save("HtmlWithCssCustomProperties.html", htmlOptions);

            // Установите в false для сравнения
            htmlOptions.EnableCssCustomProperties = false;
            workbook.Save("HtmlWithoutCssCustomProperties.html", htmlOptions);

            Console.WriteLine("Files saved with and without CSS custom properties optimization.");
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


