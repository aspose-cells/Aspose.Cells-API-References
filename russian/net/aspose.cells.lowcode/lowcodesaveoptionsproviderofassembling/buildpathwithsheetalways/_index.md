---
title: "LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSaveOptionsProviderOfAssembling. Добавлять ли всегда индекс листа или его имя в путь к файлу. Значение по умолчанию — false, то есть когда существует только один лист, индекс или имя листа и соответствующий префикс не будут добавлены в путь к файлу."
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways property

Добавлять ли всегда индекс листа или его имя в путь файла. Значение по умолчанию — false, то есть когда лист один, индекс листа (или имя) и соответствующий префикс не будут добавлены в путь файла.

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // Создать новую книгу с одним листом
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Создайте экземпляр LowCodeSaveOptionsProviderOfAssembling
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling();
            
            // Настроить параметры пути
            provider.PathHeader = "output/";
            provider.PathTail = ".xlsx";
            provider.UseSheetName = true; // Use sheet name instead of index
            provider.SheetPrefix = "_Sheet_";
            provider.SplitPartPrefix = "_Part_";
            
            // Отобразить начальное значение свойства
            Console.WriteLine("Initial BuildPathWithSheetAlways: " + provider.BuildPathWithSheetAlways);
            
            // Продемонстрировать путь к файлу без BuildPathWithSheetAlways
            string defaultPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (default): " + defaultPath);
            
            // Установить BuildPathWithSheetAlways в true
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine("\nAfter setting BuildPathWithSheetAlways to true: " + provider.BuildPathWithSheetAlways);
            
            // Продемонстрировать путь к файлу с BuildPathWithSheetAlways (даже при единственном листе)
            string updatedPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (updated): " + updatedPath);
            
            // Сохранить книгу (поведение разделения будет использовать настройки провайдера в реальных сценариях)
            workbook.Save("BuildPathWithSheetAlwaysDemo.xlsx");
        }
    }
}
```

### См. также

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


