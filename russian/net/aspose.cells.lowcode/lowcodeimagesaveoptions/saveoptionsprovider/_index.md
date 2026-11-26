---
title: "LowCodeImageSaveOptions.SaveOptionsProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeImageSaveOptions. Провайдер параметров сохранения для сохранения сгенерированных изображений"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveoptionsprovider/
---
## LowCodeImageSaveOptions.SaveOptionsProvider property

Поставщик параметров сохранения для сохранения сгенерированных изображений.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Примечания

Вывод ([`OutputFile`](../../lowcodesaveoptions/outputfile/) или [`OutputStream`](../../lowcodesaveoptions/outputstream/)), указанный этим экземпляром, не будет действовать, когда указано это свойство. Вместо этого вывод каждого сгенерированного изображения будет определяться провайдером.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Sample Image Data");
            
            // Создайте экземпляр LowCodeImageSaveOptions
            LowCodeImageSaveOptions saveOptions = new LowCodeImageSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Png;
            saveOptions.ImageOptions = new ImageOrPrintOptions();
            
            // Создать пользовательский SaveOptionsProvider
            CustomSaveOptionsProvider provider = new CustomSaveOptionsProvider();
            saveOptions.SaveOptionsProvider = provider;
            
            // Отобразите текущий SaveOptionsProvider
            Console.WriteLine("Current SaveOptionsProvider: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            // Продемонстрируйте эффект, сохраняя с разными параметрами
            workbook.Save("output_with_provider.png", saveOptions.SaveFormat);
            
            // Переключите на null-провайдер
            saveOptions.SaveOptionsProvider = null;
            Console.WriteLine("Changed SaveOptionsProvider to: " + (saveOptions.SaveOptionsProvider != null ? "Custom Provider" : "null"));
            
            workbook.Save("output_without_provider.png", saveOptions.SaveFormat);
        }
    }

    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Верните пользовательские параметры сохранения для каждой части
            return new LowCodeImageSaveOptions()
            {
                SaveFormat = SaveFormat.Jpg,  // Changed from Jpeg to Jpg
                ImageOptions = new ImageOrPrintOptions()
                {
                    Quality = 90,
                    HorizontalResolution = 300,
                    VerticalResolution = 300
                }
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Выполните очистку после сохранения
            Console.WriteLine("Finished saving part with custom options");
        }
    }
}
```

### См. также

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


