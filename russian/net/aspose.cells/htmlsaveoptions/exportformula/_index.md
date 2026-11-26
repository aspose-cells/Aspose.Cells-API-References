---
title: "HtmlSaveOptions.ExportFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, экспортировать ли формулы при сохранении файла в html. Значение по умолчанию — true. Если вы хотите импортировать полученный html в Excel, пожалуйста, оставьте значение по умолчанию"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/exportformula/
---
## HtmlSaveOptions.ExportFormula property

Указывает, экспортировать ли формулы при сохранении файла в html. Значение по умолчанию — true. Если вы хотите импортировать полученный html в Excel, пожалуйста, оставьте значение по умолчанию.

```csharp
public bool ExportFormula { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportFormulaDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте пример данных и формулу
            worksheet.Cells["A1"].PutValue("Value 1");
            worksheet.Cells["B1"].PutValue("Value 2");
            worksheet.Cells["C1"].Formula = "=A1+B1";
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].Formula = "=A2+B2";

            // Сохранить с ExportFormula = true
            HtmlSaveOptions options1 = new HtmlSaveOptions();
            options1.ExportFormula = true;
            workbook.Save("output_with_formulas.html", options1);

            // Сохранить с ExportFormula = false
            HtmlSaveOptions options2 = new HtmlSaveOptions();
            options2.ExportFormula = false;
            workbook.Save("output_without_formulas.html", options2);

            // Проверьте результаты
            string htmlWithFormulas = File.ReadAllText("output_with_formulas.html");
            string htmlWithoutFormulas = File.ReadAllText("output_without_formulas.html");

            Console.WriteLine("HTML with formulas contains formula: " + 
                htmlWithFormulas.Contains("=A2+B2"));
            Console.WriteLine("HTML without formulas contains formula: " + 
                htmlWithoutFormulas.Contains("=A2+B2"));
        }
    }
}
```

### См. также

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


