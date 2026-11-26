---
title: "AbstractLowCodeSaveOptionsProvider.Finish"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractLowCodeSaveOptionsProvider. Освобождает ресурсы после обработки текущей разделённой части"
type: docs
url: /ru/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/
---
## AbstractLowCodeSaveOptionsProvider.Finish method

Освобождает ресурсы после обработки текущей разделённой части.

```csharp
public virtual void Finish(LowCodeSaveOptions part)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| часть | LowCodeSaveOptions | параметры сохранения, используемые для текущей разделённой части. |

### Примечания

По умолчанию этот метод просто закрывает поток, указанный в [`OutputStream`](../../lowcodesaveoptions/outputstream/) напрямую (если параметры сохранения указали Stream в качестве назначения). Пользователь может переопределить этот метод, чтобы контролировать, как освобождать ресурсы в соответствии со своими требованиями и реализацией [`GetSaveOptions`](../getsaveoptions/).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo
    {
        public static void Run()
        {

            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            loadOptions.InputFile = "split.xlsx";

            // Создайте экземпляр конкретного провайдера
            var provider = new CustomLowCodeSaveOptionsProvider();

            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            splitOptions.SaveOptionsProvider = provider;
            splitOptions.LoadOptions = loadOptions;

            SpreadsheetSplitter.Process(splitOptions);
                     
          
        }
    }

    // Конкретная реализация AbstractLowCodeSaveOptionsProvider
    public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override void Finish(LowCodeSaveOptions part)
        { 
            base.Finish(part);
        }
        // Реализуйте требуемый абстрактный метод
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            LowCodeSaveOptions result = new LowCodeSaveOptions();
            result.SaveFormat = SaveFormat.Xlsx;
            result.OutputFile = partInfo.SheetName + "_split.xlsx";
            Console.WriteLine(result.OutputFile);
            return result;
        }
    }
}
```

### См. также

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


