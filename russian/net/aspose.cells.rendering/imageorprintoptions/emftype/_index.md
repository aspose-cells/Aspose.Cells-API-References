---
title: "ImageOrPrintOptions.EmfType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ImageOrPrintOptions. Получает или задаёт EmfType, который указывает формат Metafile. Значение по умолчанию — EmfPlusDual"
type: docs
url: /ru/net/aspose.cells.rendering/imageorprintoptions/emftype/
---
## ImageOrPrintOptions.EmfType property

Получает или задает EmfType, который указывает формат Metafile. Значение по умолчанию — EmfPlusDual.

```csharp
public EmfType EmfType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmfTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "EMF Type Demo";

            try
            {
                // Создайте экземпляр ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Установить тип изображения в EMF
                options.ImageType = Aspose.Cells.Drawing.ImageType.Emf;

                // Создать SheetRender с указанными параметрами
                SheetRender renderer = new SheetRender(worksheet, options);

                // Сохранить в формате EMF
                using (MemoryStream stream = new MemoryStream())
                {
                    renderer.ToImage(0, stream);

                    // Отобразить значение свойства EmfType
                    Console.WriteLine("EmfType value: " + options.EmfRenderSetting);

                    // Сохранить файл EMF
                    File.WriteAllBytes("output.emf", stream.ToArray());
                    Console.WriteLine("EMF file created successfully.");
                }
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

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


