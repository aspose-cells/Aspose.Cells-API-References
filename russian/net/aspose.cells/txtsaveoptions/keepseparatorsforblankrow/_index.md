---
title: "TxtSaveOptions.KeepSeparatorsForBlankRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtSaveOptions. Указывает, следует ли выводить разделители для пустой строки. Значение по умолчанию false, поэтому содержимое пустой строки будет пустым."
type: docs
url: /ru/net/aspose.cells/txtsaveoptions/keepseparatorsforblankrow/
---
## TxtSaveOptions.KeepSeparatorsForBlankRow property

Указывает, следует ли выводить разделители для пустой строки. Значение по умолчанию false, поэтому по умолчанию содержимое пустой строки будет пустым.

```csharp
public bool KeepSeparatorsForBlankRow { get; set; }
```

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyKeepSeparatorsForBlankRowDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Добавить некоторые данные с пустыми строками
            cells[0, 0].PutValue("a");
            cells[0, 1].PutValue("b");
            cells[3, 0].PutValue("c");
            cells[4, 1].PutValue("d");

            // Создайте параметры сохранения с KeepSeparatorsForBlankRow, установленным в true
            TxtSaveOptions options = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                KeepSeparatorsForBlankRow = true
            };

            // Сохранить книгу в CSV с параметрами
            string csvOutput = SaveAsCsv(wb, options);
            Console.WriteLine(csvOutput);
        }

        private static string SaveAsCsv(Workbook wb, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                wb.Save(stream, options);
                return Encoding.ASCII.GetString(stream.ToArray());
            }
        }
    }
}
```

### См. также

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


