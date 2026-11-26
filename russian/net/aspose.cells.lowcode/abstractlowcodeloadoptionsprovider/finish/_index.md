---
title: "AbstractLowCodeLoadOptionsProvider.Finish"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AbstractLowCodeLoadOptionsProvider. Освобождает ресурсы после обработки текущей части ввода"
type: docs
url: /ru/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/
---
## AbstractLowCodeLoadOptionsProvider.Finish method

Освобождает ресурсы после обработки текущей части входных данных.

```csharp
public virtual void Finish(LowCodeLoadOptions part)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| часть | LowCodeLoadOptions | параметры загрузки, используемые для текущей разделённой части. |

### Примечания

По умолчанию этот метод просто закрывает поток, указанный в [`InputStream`](../../lowcodeloadoptions/inputstream/) напрямую (если параметры загрузки указали Stream как источник). Пользователь может переопределить этот метод, чтобы контролировать освобождение ресурсов в соответствии со своими требованиями и реализацией [`Current`](../current/).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderMethodFinishWithLowCodeLoadOptionsDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };

            CustomLoadOptionsProvider provider = new CustomLoadOptionsProvider(files);

            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "result.xlsx";
            saveOptions.SaveFormat = SaveFormat.Xlsx;

            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            mergeOptions.LoadOptionsProvider = provider;
            mergeOptions.SaveOptions = saveOptions;

            SpreadsheetMerger.Process(mergeOptions);
        }
    }

    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {       

        public IEnumerator fileIter;
        public CustomLoadOptionsProvider(string[] files)
        {
            fileIter = files.GetEnumerator();
            current = new LowCodeLoadOptions();
        }
        private LowCodeLoadOptions current;

        public override LowCodeLoadOptions Current => current;

        public override bool MoveNext()
        {
            if (fileIter.MoveNext())
            {
                current = new LowCodeLoadOptions();
                current.InputFile = fileIter.Current.ToString();
                return true;
            }
            
            return false;
        }

        public override void Finish(LowCodeLoadOptions part)
        {
            base.Finish(part);
        }
    }
}
```

### См. также

* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


