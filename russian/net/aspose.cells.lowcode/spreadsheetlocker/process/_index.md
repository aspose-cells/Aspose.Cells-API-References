---
title: "SpreadsheetLocker.Process"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SpreadsheetLocker. Блокирует файл электронной таблицы с указанными настройками"
type: docs
url: /ru/net/aspose.cells.lowcode/spreadsheetlocker/process/
---
## Process(string, string, string, string) {#process_3}

Блокирует файл электронной таблицы с указанными настройками.

```csharp
public static void Process(string templateFile, string resultFile, string openPassword, 
    string writePassword)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| templateFile | String | Файл шаблона, который будет заблокирован |
| resultFile | String | Полученный файл |
| openPassword | String | Пароль для шифрования файла |
| writePassword | String | Пароль для защиты от изменения электронной таблицы |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class SpreadsheetLockerMethodProcessWithStringStringStringStringDemo
    {
        public static void Run()
        {           
            string templatePath = "template.xlsx";            
            // Подготовить путь к результирующему файлу
            string resultPath = "secured_spreadsheet.xlsx";

            try
            {
                // Выполнить метод Process с параметрами строкового типа напрямую, используя тип
                SpreadsheetLocker.Process(
                    templateFile: templatePath,
                    resultFile: resultPath,
                    openPassword: "Open@123",
                    writePassword: "Write@456"
                );

                Console.WriteLine($"Spreadsheet secured successfully. Saved to: {Path.GetFullPath(resultPath)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error securing spreadsheet: {ex.Message}");
            }
            finally
            {
                // Очистить временный шаблон
                if (File.Exists(templatePath))
                {
                    File.Delete(templatePath);
                }
            }
        }
    }
}
```

### См. также

* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string) {#process_1}

Блокирует файл электронной таблицы с указанными настройками.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Параметры ввода и загрузки |
| saveOptions | LowCodeSaveOptions | Параметры вывода и сохранения |
| openPassword | String | Пароль для шифрования файла |
| writePassword | String | Пароль для защиты от изменения электронной таблицы |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo
    {
        public static void Run()
        {
            
            // Обработать таблицу с паролями блокировки/разблокировки
            SpreadsheetLocker.Process(
                new LowCodeLoadOptions() { InputFile = "input.xlsx" },
                new LowCodeSaveOptions() 
                { 
                    OutputFile = "output_locked.xlsx" 
                }, 
                "123456", 
                "234567");
        }
    }
}
```

### См. также

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, string, string, string, ProtectionType) {#process_2}

Блокирует файл электронной таблицы с указанными настройками.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    string openPassword, string writePassword, string workbookPassword, ProtectionType workbookType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Параметры ввода и загрузки |
| saveOptions | LowCodeSaveOptions | Параметры вывода и сохранения |
| openPassword | String | Пароль для шифрования файла |
| writePassword | String | Пароль для защиты от изменения электронной таблицы |
| workbookPassword | String | Пароль для защиты рабочей книги |
| workbookType | ProtectionType | Тип защиты для защиты рабочей книги |

### См. также

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeLoadOptions, LowCodeSaveOptions, AbstractLowCodeProtectionProvider) {#process}

Блокирует файл электронной таблицы с указанными настройками.

```csharp
public static void Process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, 
    AbstractLowCodeProtectionProvider provider)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| loadOptions | LowCodeLoadOptions | Параметры ввода и загрузки |
| saveOptions | LowCodeSaveOptions | Параметры вывода и сохранения |
| провайдер | AbstractLowCodeProtectionProvider | Реализация для предоставления настроек защиты |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetLockerMethodProcessWithLowCodeLoadOptionsLowCodeSaveODemo1
    {
        public static void Run()
        {
           
            // Подготовить LowCodeLoadOptions
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "input.xlsx";

            // Подготовить LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            saveOptions.OutputFile = "output.xlsx";

            // Создать пользовательского поставщика защиты
            CustomProtectionProvider provider = new CustomProtectionProvider();

            try
            {
                // Вызвать статический метод Process с указанными параметрами
                SpreadsheetLocker.Process(loadOptions, saveOptions, provider);

                Console.WriteLine("Spreadsheet processed and protected successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error processing spreadsheet: {ex.Message}");
            }

        }

        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override string GetOpenPassword()
            {
                return "open123";
            }

            public override string GetWritePassword()
            {
                return "write123";
            }

            public override string GetWorkbookPassword()
            {
                return "workbook123";
            }

            public override ProtectionType GetWorkbookProtectionType()
            {
                return ProtectionType.All;
            }
        }
    }
}
```

### См. также

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeProtectionProvider](../../abstractlowcodeprotectionprovider/)
* class [SpreadsheetLocker](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


