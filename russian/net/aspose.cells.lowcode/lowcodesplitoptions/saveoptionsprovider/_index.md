---
title: "LowCodeSplitOptions.SaveOptionsProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LowCodeSplitOptions. Поставщик параметров сохранения для сохранения разделённых частей"
type: docs
url: /ru/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/
---
## LowCodeSplitOptions.SaveOptionsProvider property

Провайдер параметров сохранения для сохранения разделённых частей.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Примечания

Если это свойство указано, [`SaveOptions`](../saveoptions/) не оказывает влияния, потому что вывод каждой разделённой части будет задан поставщиком.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните некоторыми образцовыми данными
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // Создать экземпляр LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // Отобразить текущее значение SaveOptionsProvider (по умолчанию null)
            Console.WriteLine("Current SaveOptionsProvider value: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Создать пользовательский SaveOptionsProvider
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // Продемонстрировать эффект установки SaveOptionsProvider
            // В реальном сценарии это будет использоваться при разделении файлов
            Console.WriteLine("After setting SaveOptionsProvider: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Сохранить книгу (хотя разделение здесь не продемонстрировано)
            workbook.Save("PropertySaveOptionsProviderDemo.xlsx");
        }
    }

    // Пользовательская реализация AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Создать пользовательские параметры сохранения для каждой разделённой части
            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            return options;
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Выполнить очистку после сохранения каждой части
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### См. также

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


