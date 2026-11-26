---
title: "AbstractLowCodeSaveOptionsProvider.GetSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractLowCodeSaveOptionsProvider. Получает параметры сохранения, из которых берутся настройки вывода для текущей разделённой части. Возврат null означает пропустить данную часть."
type: docs
url: /ru/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/
---
## AbstractLowCodeSaveOptionsProvider.GetSaveOptions method

Получает параметры сохранения, из которых берутся настройки вывода для текущей разделённой части. Возврат null означает пропустить данную часть.

```csharp
public abstract LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using AsposeCellsExamples.AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // Создайте экземпляр конкретного провайдера
            var provider = new CustomSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
        }
    }

    // Пользовательская реализация AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // Создайте пользовательские параметры сохранения на основе информации о части
            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = $"Part_{partInfo.PartIndex}_Sheet_{partInfo.SheetName}.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;

        }
    }
}
```

### См. также

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


