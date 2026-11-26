---
title: "SplitPartInfo.SheetName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SplitPartInfo. Имя листа, в котором находится текущая часть"
type: docs
url: /ru/net/aspose.cells.lowcode/splitpartinfo/sheetname/
---
## SplitPartInfo.SheetName property

Имя листа, в котором находится текущая часть.

```csharp
public string SheetName { get; }
```

### Примечания

Может быть null в некоторых ситуациях, например при рендеринге всей книги в изображение TIFF.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using AsposeCellsExamples.AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo;
    using System;
    using System.Reflection;

    public class SplitPartInfoPropertySheetNameDemo
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

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


