---
title: "Класс LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfPlaceHolders класс. Реализация, предоставляющая параметры сохранения, которые сохраняют разделённые части в файлы, а путь результирующего файла определяется с помощью заполнителей"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders class

Реализация, предоставляющая параметры сохранения, которые сохраняют разделённые части в файлы, а путь результирующего файла определяется с помощью заполнителей.

```csharp
public class LowCodeSaveOptionsProviderOfPlaceHolders : AbstractLowCodeSaveOptionsProvider
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders](lowcodesaveoptionsproviderofplaceholders/)(string) | Создает экземпляр для предоставления параметров сохранения в соответствии с указанными шаблонами. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/) { get; set; } | Определяет, добавлять ли индекс или имя листа к пути файла всегда. Значение по умолчанию — false, то есть когда листов только один, индекс листа, его имя и соответствующий префикс([`SheetNamePrefix`](./sheetnameprefix/)) не будут добавлены к пути файла. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/) { get; set; } | Определяет, добавлять ли всегда индекс части разбиения к пути файла. Значение по умолчанию — false, то есть когда часть разбиения одна, её индекс и соответствующий префикс([`SplitPartPrefix`](./splitpartprefix/)) не будут добавлены к пути файла. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/) { get; set; } | Шаблон для создания экземпляра параметров сохранения в [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/) { get; set; } | Смещение индекса листа между тем, что используется в пути файла, и его фактическим значением ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetIndexPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/) { get; set; } | Префикс для индекса листа. |
| [SheetNamePrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/) { get; set; } | Префикс для индекса листа. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/) { get; set; } | Смещение индекса части разделения между тем, что используется в пути файла, и его фактическим значением ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/) { get; set; } | Префикс для индекса части разделения. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Освобождает ресурсы после обработки текущей части разделения. (Наследовано от [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/)(SplitPartInfo) | Получает параметры сохранения, из которых берутся настройки вывода для текущей части разделения. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;

    public class LowCodeClassLowCodeSaveOptionsProviderOfPlaceHoldersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполнить лист образцовыми данными
            for (int i = 0; i < 250; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // Создать провайдер с шаблоном пути, содержащим заполнители
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_Sheet_{sheet}_Part_{split}.xlsx");
            
            // Настроить свойства провайдера
            provider.SheetIndexOffset = 1;
            provider.SplitPartIndexOffset = 1;
            provider.SheetIndexPrefix = "S";
            provider.SplitPartPrefix = "P";
            provider.BuildPathWithSheetAlways = true;
            provider.BuildPathWithSplitPartAlways = true;

            // Настроить шаблон параметров сохранения
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Настроить параметры изображения или печати для раздельного рендеринга
            var imgOrPrintOptions = new ImageOrPrintOptions
            {
                SaveFormat = SaveFormat.Pdf,
                OnePagePerSheet = false,
                PageIndex = 0,
                PageCount = 1
            };

            // Создать рендер листа с конфигурацией разбиения
            var sheetRender = new SheetRender(worksheet, imgOrPrintOptions);
            sheetRender.ToImage(0, "output"); // This would normally split and save using provider
        }
    }
}
```

### См. также

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


