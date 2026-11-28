---
title: "AbstractLowCodeLoadOptionsProvider.MoveNext"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AbstractLowCodeLoadOptionsProvider yöntemi. Daha fazla girdi olup olmadığını kontrol eder"
type: docs
url: /tr/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/
---
## AbstractLowCodeLoadOptionsProvider.MoveNext method

Daha fazla giriş olup olmadığını kontrol eder.

```csharp
public abstract bool MoveNext()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderMethodMoveNextDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };
            // AbstractLowCodeLoadOptionsProvider'ı uygulayan özel bir sağlayıcı oluştur
            MultiFileProvider provider = new MultiFileProvider(files);

            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
            saveOptions.OutputFile = "result.xlsx";
            saveOptions.SaveFormat = SaveFormat.Xlsx;

            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            mergeOptions.LoadOptionsProvider = provider;
            mergeOptions.SaveOptions = saveOptions;

            SpreadsheetMerger.Process(mergeOptions);

        }

        private class MultiFileProvider : AbstractLowCodeLoadOptionsProvider
        {
            public IEnumerator fileIter;
            public MultiFileProvider(string[] files)
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
}
```

### Ayrıca Bakınız

* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


