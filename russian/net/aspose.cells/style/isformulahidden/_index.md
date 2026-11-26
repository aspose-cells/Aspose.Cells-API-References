---
title: "Style.IsFormulaHidden"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Представляет, будет ли формула скрыта, когда лист защищён"
type: docs
url: /ru/net/aspose.cells/style/isformulahidden/
---
## Style.IsFormulaHidden property

Представляет, будет ли формула скрыта, когда лист защищён.

```csharp
public bool IsFormulaHidden { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFormulaHiddenDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создайте стиль с IsFormulaHidden, установленным в true
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;
            
            // Применить стиль к ячейке
            cells["A1"].SetStyle(style);
            cells["A1"].Formula = "=1+1";

            // Создайте другой стиль с IsFormulaHidden, установленным в false
            Style style2 = workbook.CreateStyle();
            style2.IsFormulaHidden = false;
            
            // Примените второй стиль к другой ячейке
            cells["B1"].SetStyle(style2);
            cells["B1"].Formula = "=2+2";

            // Защитите лист, чтобы увидеть эффект
            worksheet.Protect(ProtectionType.All, "password", null);

            // Сохраните книгу
            workbook.Save("IsFormulaHiddenDemo.xlsx");

            Console.WriteLine("Workbook saved with IsFormulaHidden examples.");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


