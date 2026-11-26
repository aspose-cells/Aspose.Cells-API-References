---
title: "LoadOptions.PreservePaddingSpacesInFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Указывает, следует ли сохранять пробелы и разрывы строк, которые добавлены между токенами формулы при получении и установке формул. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/loadoptions/preservepaddingspacesinformula/
---
## LoadOptions.PreservePaddingSpacesInFormula property

Указывает, следует ли сохранять пробелы и переносы строк, добавленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.

```csharp
public bool PreservePaddingSpacesInFormula { get; set; }
```

### Примечания

После загрузки книги из файла шаблона с этой опцией, [`PreservePaddingSpaces`](../../formulasettings/preservepaddingspaces/) будет установлена в то же значение, что и это свойство.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPreservePaddingSpacesInFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Включить сохранение пробелов‑заполнителей в формулах
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = true;
            
            // Получить доступ к первому листу и задать формулу с пробелами‑заполнителями
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            string formulaWithSpaces = "= IF(1 <>2, 2, 1)";
            cell.Formula = formulaWithSpaces;
            
            // Сохранить и перезагрузить книгу с опцией PreservePaddingSpacesInFormula
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx)
            {
                PreservePaddingSpacesInFormula = true
            };
            
            Workbook reloadedWorkbook = new Workbook(outputPath, loadOptions);
            Worksheet reloadedWorksheet = reloadedWorkbook.Worksheets[0];
            
            // Проверить, что формула сохранила пробелы после перезагрузки
            Console.WriteLine("Original formula: " + formulaWithSpaces);
            Console.WriteLine("Reloaded formula: " + reloadedWorksheet.Cells["A1"].Formula);
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


