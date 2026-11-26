---
title: "HtmlSaveOptions.OfficeMathOutputMode"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Указывает, как объекты OfficeMath экспортируются в HTML. Значение по умолчанию — Image"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/officemathoutputmode/
---
## HtmlSaveOptions.OfficeMathOutputMode property

Указывает, как объекты OfficeMath экспортируются в HTML, значение по умолчанию — Image.

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputMode { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class HtmlSaveOptionsPropertyOfficeMathOutputModeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var cell = worksheet.Cells["A1"];
            
            // Добавьте форму уравнения, используя доступный метод
            TextBox equationTextBox = worksheet.Shapes.AddEquation(cell.Row, 0, cell.Column, 0, 100, 50);
            equationTextBox.Text = "1/2"; // Set equation text

            // Создать параметры сохранения HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();

            // Отобразите и измените OfficeMathOutputMode
            Console.WriteLine("Initial OfficeMathOutputMode: " + saveOptions.OfficeMathOutputMode);
            workbook.Save("OfficeMathDefault.html", saveOptions);

            saveOptions.OfficeMathOutputMode = HtmlOfficeMathOutputType.MathML;
            Console.WriteLine("Modified OfficeMathOutputMode: " + saveOptions.OfficeMathOutputMode);
            workbook.Save("OfficeMathMathML.html", saveOptions);
        }
    }
}
```

### См. также

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


