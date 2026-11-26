---
title: "PdfSaveOptions.ImageType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. Представляет тип изображения при преобразовании диаграммы и фигуры"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/imagetype/
---
## PdfSaveOptions.ImageType property

Представляет тип изображения при преобразовании диаграммы и фигуры.

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ImageType { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого диаграммы и фигуры всегда рендерятся как векторные элементы (например, точка, линия) для обеспечения качества отображения. Это свойство будет удалено через 12 месяцев, начиная с июня 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing.Imaging;

    public class PdfSaveOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Создать пример листа с некоторыми данными
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for PDF Export";
            worksheet.Cells["A2"].Value = "Demonstrating ImageType Property";

            try
            {
                // Создайте параметры сохранения PDF
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Отобразить значение ImageType по умолчанию
                Console.WriteLine("Default ImageType: " + saveOptions.ImageType);

                // Установить другое значение ImageType
                saveOptions.ImageType = ImageFormat.Png;
                Console.WriteLine("Updated ImageType: " + saveOptions.ImageType);

                // Сохранить рабочую книгу как PDF с указанным ImageType
                workbook.Save("ImageTypeDemo.pdf", saveOptions);

                Console.WriteLine("PDF saved with ImageType setting applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


