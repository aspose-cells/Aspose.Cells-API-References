---
title: "TxtLoadOptions.TreatQuotePrefixAsValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TxtLoadOptions. Указывает, следует ли воспринимать начальный одинарный апостроф как часть значения ячейки. По умолчанию true. Если false, начальный одинарный апостроф будет удалён из значения соответствующей ячейки, и QuotePrefix будет установлен в true для этой ячейки."
type: docs
url: /ru/net/aspose.cells/txtloadoptions/treatquoteprefixasvalue/
---
## TxtLoadOptions.TreatQuotePrefixAsValue property

Указывает, следует ли воспринимать начальный одинарный апостроф как часть значения ячейки. По умолчанию true. Если false, начальный одинарный апостроф будет удалён из значения соответствующей ячейки, и [`QuotePrefix`](../../style/quoteprefix/) будет установлен в true для этой ячейки.

```csharp
public bool TreatQuotePrefixAsValue { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTreatQuotePrefixAsValueDemo
    {
        public static void Run()
        {
            // Создать пример данных CSV с префиксами кавычек
            string csvData = "ID,Name,Value\n1,\"'Apple\",100\n2,\"'Orange\",200";
            string filePath = "test.csv";

            // Сохранить данные CSV в файл
            File.WriteAllText(filePath, csvData);

            // Сценарий 1: TreatQuotePrefixAsValue = false (по умолчанию)
            var loadOptions1 = new TxtLoadOptions();
            loadOptions1.TreatQuotePrefixAsValue = false;
            
            var workbook1 = new Workbook(filePath, loadOptions1);
            var worksheet1 = workbook1.Worksheets[0];
            Console.WriteLine("TreatQuotePrefixAsValue = false:");
            Console.WriteLine("Cell B2 value: " + worksheet1.Cells["B2"].Value); // Will show 'Apple (quote treated as formatting)

            // Сценарий 2: TreatQuotePrefixAsValue = true
            var loadOptions2 = new TxtLoadOptions();
            loadOptions2.TreatQuotePrefixAsValue = true;
            
            var workbook2 = new Workbook(filePath, loadOptions2);
            var worksheet2 = workbook2.Worksheets[0];
            Console.WriteLine("\nTreatQuotePrefixAsValue = true:");
            Console.WriteLine("Cell B2 value: " + worksheet2.Cells["B2"].Value); // Will show 'Apple (quote treated as value)

            // Очистить
            File.Delete(filePath);
        }
    }
}
```

### См. также

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


