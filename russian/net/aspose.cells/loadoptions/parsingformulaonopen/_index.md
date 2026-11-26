---
title: "LoadOptions.ParsingFormulaOnOpen"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Указывает, выполняется ли разбор формул при чтении файла"
type: docs
url: /ru/net/aspose.cells/loadoptions/parsingformulaonopen/
---
## LoadOptions.ParsingFormulaOnOpen property

Указывает, следует ли разбирать формулу при чтении файла.

```csharp
public bool ParsingFormulaOnOpen { get; set; }
```

### Примечания

Применяется только к файлам Excel Xlsx, Xltx, Xltm и Xlsm, потому что формулы в файлах хранятся в виде строковой формулы.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingFormulaOnOpenDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки
            LoadOptions loadOptions = new LoadOptions();
            
            // Установите ParsingFormulaOnOpen в false, чтобы пропустить разбор формул при загрузке
            loadOptions.ParsingFormulaOnOpen = false;
            
            // Загрузите рабочую книгу с указанными параметрами
            Workbook workbook = new Workbook("example.xlsm", loadOptions);
            
            // Получите доступ к листу и продемонстрируйте, что разбор формул был пропущен
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Console.WriteLine("Cell A1 formula: " + cell.Formula);
            Console.WriteLine("Cell A1 value: " + cell.Value);
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


