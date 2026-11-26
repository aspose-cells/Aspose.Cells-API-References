---
title: "MarkdownLoadOptions.HasFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство MarkdownLoadOptions. Указывает, является ли текст формулой, если он начинается с"
type: docs
url: /ru/net/aspose.cells/markdownloadoptions/hasformula/
---
## MarkdownLoadOptions.HasFormula property

Указывает, является ли текст формулой, если он начинается с "=".

```csharp
public bool HasFormula { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Создать экземпляр MarkdownLoadOptions
                MarkdownLoadOptions options = new MarkdownLoadOptions();

                // Отобразить значение по умолчанию свойства HasFormula
                Console.WriteLine($"Default HasFormula value: {options.HasFormula}");

                // Установить HasFormula в true
                options.HasFormula = true;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Установить HasFormula в false
                options.HasFormula = false;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Создать workbook с примерным содержимым markdown
                Workbook workbook = new Workbook();

                // Сохранить workbook, чтобы продемонстрировать возможность использования опций
                workbook.Save("HasFormulaDemo.xlsx");

                Console.WriteLine("HasFormula property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [MarkdownLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


