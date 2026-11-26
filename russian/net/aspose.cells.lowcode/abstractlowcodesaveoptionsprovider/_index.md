---
title: "Класс AbstractLowCodeSaveOptionsProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.LowCode.AbstractLowCodeSaveOptionsProvider. Реализация, предоставляющая несколько вариантов сохранения для процессов, требующих множественных выводов. Например, функция SpreadsheetSplitter требует нескольких назначений для сохранения разделённых файлов."
type: docs
url: /ru/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/
---
## AbstractLowCodeSaveOptionsProvider class

Реализация, предоставляющая несколько вариантов сохранения для процессов, требующих множественных выводов. Например, функция [`SpreadsheetSplitter`](../spreadsheetsplitter/) требует нескольких назначений для сохранения разделённых файлов.

```csharp
public abstract class AbstractLowCodeSaveOptionsProvider
```

## Методы

| Имя | Описание |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Освобождает ресурсы после обработки текущей разделённой части. |
| abstract [GetSaveOptions](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/)(SplitPartInfo) | Получает параметры сохранения, из которых берутся настройки вывода для текущей разделённой части. Возврат null означает пропустить данную часть. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeSaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Создайте пользовательского провайдера, расширив AbstractLowCodeSaveOptionsProvider
            var customProvider = new CustomSaveOptionsProvider();

            // Создайте книгу и лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните некоторыми данными
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // Создайте информацию о разделённой части — в реальном использовании она будет получена из API
            // Поскольку мы не можем создать её напрямую, мы просто передадим null для демонстрации
            SplitPartInfo splitPartInfo = null;
            
            // Получить параметры сохранения от провайдера
            LowCodeSaveOptions saveOptions = customProvider.GetSaveOptions(splitPartInfo);
            
            // Настроить параметры сохранения (пример)
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            
            // Продемонстрировать завершение процесса
            customProvider.Finish(saveOptions);
            
            // Сохранить книгу (не напрямую связано с провайдером, только для демонстрации)
            workbook.Save("LowCodeSaveOptionsDemo.xlsx");
        }
    }

    // Пользовательская реализация AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Создать и вернуть пользовательские параметры сохранения на основе информации о части
            return new LowCodeSaveOptions()
            {
                SaveFormat = SaveFormat.Xlsx
                // Удалён CachedFileFolder, так как он не существует в LowCodeSaveOptions
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Логика очистки или завершения здесь
            Console.WriteLine("Save operation completed for part");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


