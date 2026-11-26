---
title: "AbstractLowCodeLoadOptionsProvider.Current"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AbstractLowCodeLoadOptionsProvider. Получает параметры загрузки, из которых загружаются данные текущей обрабатываемой части"
type: docs
url: /ru/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/
---
## AbstractLowCodeLoadOptionsProvider.Current property

Получает параметры загрузки, из которых загружать данные текущей обрабатываемой части.

```csharp
public abstract LowCodeLoadOptions Current { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.Collections;

    public class AbstractLowCodeLoadOptionsProviderPropertyCurrentDemo
    {
        public static void Run()
        {
            string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };
            // Инициализировать пользовательского провайдера с нашими параметрами загрузки
            CustomProvider provider = new CustomProvider(files);
            
            int counter = 1;
            while (provider.MoveNext())
            {
                // Получить свойство Current, чтобы получить активные параметры загрузки
                Console.WriteLine($"Processing set {counter}");
                    
                // Создать рабочую книгу, используя входной файл/поток текущих параметров загрузки
                Workbook workbook;
                if (provider.Current.InputFile != null)
                {
                    workbook = new Workbook(provider.Current.InputFile);
                }
                else if (provider.Current.InputStream != null)
                {
                    workbook = new Workbook(provider.Current.InputStream);
                }
                else
                {
                    workbook = new Workbook();
                }

                Worksheet worksheet = workbook.Worksheets[0];

                // Продемонстрировать влияние опции, удалённое из‑за отсутствующего свойства
                worksheet.Cells["A1"].Value = "Sample Value";

                // Сохранить результат
                workbook.Save($"CurrentDemo_{counter}.xlsx");
                counter++;
            }
        }
    }

    // Реализация пользовательского провайдера с IDisposable
    public class CustomProvider : AbstractLowCodeLoadOptionsProvider
    {
        
        public IEnumerator fileIter;

        public CustomProvider(string[] files)
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


