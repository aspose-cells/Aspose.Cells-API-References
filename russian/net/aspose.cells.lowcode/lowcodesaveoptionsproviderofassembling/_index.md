---
title: "Класс LowCodeSaveOptionsProviderOfAssembling"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfAssembling class. Реализация, предоставляющая параметры сохранения, которые сохраняют разделённые части в файлы, а путь результирующего файла называется так, как могут содержать каталоги PathHeaderSheetPrefixSheetIndexor SheetName SplitPartPrefixSplitPartIndexPathTail"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/
---
## LowCodeSaveOptionsProviderOfAssembling class

Реализация, предоставляющая параметры сохранения, которые сохраняют разделённые части в файлы, а путь результирующего файла называется так (может содержать каталоги): [`PathHeader`](./pathheader/)+[`SheetPrefix`](./sheetprefix/)+SheetIndex(или SheetName) +[`SplitPartPrefix`](./splitpartprefix/)+SplitPartIndex+[`PathTail`](./pathtail/).

```csharp
public class LowCodeSaveOptionsProviderOfAssembling : AbstractLowCodeSaveOptionsProvider
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling](lowcodesaveoptionsproviderofassembling/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/) { get; set; } | Добавлять ли всегда индекс листа или его имя в путь файла. Значение по умолчанию — false, то есть когда лист один, индекс листа (или имя) и соответствующий префикс не будут добавлены в путь файла. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/) { get; set; } | Добавлять ли всегда индекс части разделения в путь файла. Значение по умолчанию — false, то есть когда часть разделения одна, её индекс и соответствующий префикс не будут добавлены в путь файла. |
| [PathHeader](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/) { get; set; } | Часть заголовка (до добавленного содержимого листа и части разделения) пути файла. |
| [PathTail](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/) { get; set; } | Конечная часть (после последовательных номеров) пути файла. Она должна включать расширение имени файла. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/) { get; set; } | Шаблон для создания экземпляра параметров сохранения в [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/) { get; set; } | Смещение индекса листа между тем, что используется в пути файла, и его фактическим значением ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/) { get; set; } | Префикс для индекса листа. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/) { get; set; } | Смещение индекса части разделения между тем, что используется в пути файла, и его фактическим значением ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/) { get; set; } | Префикс для индекса части разделения. |
| [UseSheetName](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/) { get; set; } | Создавать ли путь файла с именем листа вместо его индекса. Значение по умолчанию — false. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Освобождает ресурсы после обработки текущей части разделения. (Наследовано от [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/)(SplitPartInfo) | Получает параметры сохранения, из которых берутся настройки вывода для текущей части разделения. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;

    public class LowCodeClassLowCodeSaveOptionsProviderOfAssemblingDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data {i + 1}";
            }

            // Инициализировать и настроить провайдер параметров сохранения
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitOutput/",
                PathTail = "_Part.xlsx",
                UseSheetName = true,
                SheetPrefix = "SHEET-",
                SplitPartPrefix = "PART-",
                BuildPathWithSheetAlways = true,
                BuildPathWithSplitPartAlways = true,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Настроить параметры сохранения XLSX с разделением, используя LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Сохранить рабочую книгу с включёнными провайдером параметрами, используя правильный формат сохранения
            workbook.Save("LowCodeSaveOptionsProviderOfAssemblingDemo_Output.xlsx", saveOptions.SaveFormat);
        }
    }
}
```

### См. также

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


