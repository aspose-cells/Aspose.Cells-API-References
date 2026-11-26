---
title: "TxtLoadOptions.TextQualifier"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtLoadOptions. Указывает текстовый квалификатор для значений ячеек. Квалификатор по умолчанию —"
type: docs
url: /ru/net/aspose.cells/txtloadoptions/textqualifier/
---
## TxtLoadOptions.TextQualifier property

Указывает текстовый квалификатор для значений ячеек. Квалификатор по умолчанию — '"'.

```csharp
public char TextQualifier { get; set; }
```

### Примечания

При установке этого свойства, [`HasTextQualifier`](../hastextqualifier/) будет автоматически установлено в true.

### Примеры

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTextQualifierDemo
    {
        public static void Run()
        {
            // Создайте экземпляр TxtLoadOptions для CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                HasTextQualifier = true,
                TextQualifier = '\"'
            };

            // Создайте пример CSV-данных с текстовыми квалификаторами
            string csvData = "Name,Age,City\n\"John Doe\",30,\"New York\"\n\"Jane Smith\",25,\"San Francisco\"";
            
            // Сохраните примерные данные во временный файл
            string tempFile = "temp.csv";
            System.IO.File.WriteAllText(tempFile, csvData);

            // Загрузите CSV-файл с указанными параметрами
            Workbook workbook = new Workbook(tempFile, loadOptions);

            // Сохраните Workbook в файл Excel
            workbook.Save("TextQualifierDemo.xlsx");

            // Очистите временный файл
            System.IO.File.Delete(tempFile);
        }
    }
}
```

### См. также

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


