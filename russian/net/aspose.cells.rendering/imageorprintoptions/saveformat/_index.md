---
title: "ImageOrPrintOptions.SaveFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Возвращает или задает тип формата выходного файла. Поддерживает Tiff/XPS."
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/saveformat/
---
## ImageOrPrintOptions.SaveFormat property

Возвращает или задает тип формата выходного файла. Поддерживает Tiff/XPS.

```csharp
[Obsolete("For Tiff/Svg, use ImageType; For Xps, use Workbook.Save(string, SaveOptions) with XpsSaveOptions")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SaveFormat SaveFormat { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него для Tiff/Svg используйте [`ImageType`](../imagetype/); для Xps используйте [`Save`](../../../aspose.cells/workbook/save/) с [`XpsSaveOptions`](../../../aspose.cells/xpssaveoptions/). Это свойство будет удалено через 12 месяцев, начиная с августа 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Создайте новую рабочую книгу и заполните её примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells SaveFormat Demonstration");
            
            // Создайте экземпляр ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Отобразить начальное значение SaveFormat
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // Установите SaveFormat в TIFF и отрисуйте лист
            options.SaveFormat = SaveFormat.Tiff;
            SheetRender tiffRenderer = new SheetRender(worksheet, options);
            using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
            {
                tiffRenderer.ToTiff(tiffStream);
            }
            Console.WriteLine("Rendered worksheet to TIFF format");

            // Измените SaveFormat на XPS и отрисуйте снова
            options.SaveFormat = SaveFormat.Xps;
            SheetRender xpsRenderer = new SheetRender(worksheet, options);
            using (FileStream xpsStream = new FileStream("output.xps", FileMode.Create))
            {
                // Примечание: SheetRender не поддерживает формат XPS. Вместо этого будет сохранено в формате изображения.
                xpsRenderer.ToImage(0, xpsStream);
            }
            Console.WriteLine("Rendered worksheet to XPS format");
        }
    }
}
```

### См. также

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


