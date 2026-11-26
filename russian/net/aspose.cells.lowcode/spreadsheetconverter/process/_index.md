---
title: "SpreadsheetConverter.Process"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SpreadsheetConverter. Преобразует заданный шаблонный файл между форматами электронных таблиц"
type: docs
url: /ru/net/aspose.cells.lowcode/spreadsheetconverter/process/
---
## Process(string, string) {#process_1}

Преобразует указанный файл шаблона между форматами файлов электронных таблиц.

```csharp
public static void Process(string templateFile, string resultFile)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| templateFile | String | Файл шаблона для преобразования |
| resultFile | String | Полученный файл |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithStringStringDemo
    {
        public static void Run()
        {
            SpreadsheetConverter.Process("file1.xlsx", "SpreadsheetConverterMethodProcessWithStringStringDemo.xlsb");
        }
    }
}
```

### См. также

* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions) {#process}

Преобразует между различными форматами файлов электронных таблиц.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Параметры ввода и загрузки |
| saveOptions | LowCodeSaveOptions | Параметры вывода и сохранения |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            // Создать параметры загрузки с входным файлом
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "file1.xlsx";

            // Создать параметры сохранения с выходным файлом
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "SpreadsheetConverterMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo.xlsx";

            // Выполнить преобразование
            SpreadsheetConverter.Process(loadOptions, saveOptions);
        }
    }
}
```

### См. также

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetConverter](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


