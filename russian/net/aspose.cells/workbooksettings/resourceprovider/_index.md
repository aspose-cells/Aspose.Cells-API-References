---
title: "WorkbookSettings.ResourceProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Получает и задает поставщика потоков для внешних ресурсов, например загрузку данных изображения для картинки типа LinkToFile"
type: docs
url: /ru/net/aspose.cells/workbooksettings/resourceprovider/
---
## WorkbookSettings.ResourceProvider property

Получает и задает поставщика потоков для внешних ресурсов, например загрузку данных изображения для картинки типа "LinkToFile".

```csharp
public IStreamProvider ResourceProvider { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyResourceProviderDemo
    {
        public static void Run()
        {
            // Создать пример рабочей книги
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте пример фигуры, чтобы продемонстрировать поставщика ресурсов
            worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
            
            // Установите поставщика ресурсов
            workbook.Settings.ResourceProvider = new MemoryStreamProvider();
            
            // Сохраните фигуру как изображение, используя поставщика ресурсов
            string outputPath = "output_shape.png";
            worksheet.Shapes[0].ToImage(outputPath, new ImageOrPrintOptions());
            
            Console.WriteLine("Shape saved as image using ResourceProvider.");
        }
    }

    public class MemoryStreamProvider : IStreamProvider
    {
        public void CloseStream(StreamProviderOptions options)
        {
            options.Stream.Close();
        }

        public void InitStream(StreamProviderOptions options)
        {
            options.Stream = new FileStream(options.DefaultPath, FileMode.Create);
        }
    }
}
```

### См. также

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


