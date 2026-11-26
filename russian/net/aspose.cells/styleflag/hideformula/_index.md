---
title: "StyleFlag.HideFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройка Hide formula будет применена"
type: docs
url: /ru/net/aspose.cells/styleflag/hideformula/
---
## StyleFlag.HideFormula property

Настройка скрытия формулы будет применена.

```csharp
public bool HideFormula { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyHideFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell a1 = worksheet.Cells["A1"];
            // Добавьте формулу в ячейку A1
            a1.Formula = "=1+2";
            a1.Value = 3; // Display value

            // Создайте флаг стиля с HideFormula, установленным в true
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HideFormula = true;

            // Создайте стиль и установите IsFormulaHidden в true
            Style style = workbook.CreateStyle();
            style.IsFormulaHidden = true;

            // Примените стиль к ячейке A1 с флагом стиля
            a1.SetStyle(style, styleFlag);

            // Защитите лист, чтобы увидеть эффект HideFormula
            worksheet.Protection.AllowEditingObject = true;
            worksheet.Protection.AllowEditingContent = false;
            worksheet.Protection.Password = "password";

            // Сохраните книгу
            workbook.Save("PropertyHideFormulaDemo.xlsx");

            // Проверьте, что формула скрыта
            Console.WriteLine("Formula in A1: " + a1.Formula);
            Console.WriteLine("Is formula hidden? " + a1.GetStyle().IsFormulaHidden);
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


