---
title: "HtmlSaveOptions.SheetSet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство HtmlSaveOptions. Получает или задает листы для рендеринга. По умолчанию — все видимые листы в книге Visible"
type: docs
url: /ru/net/aspose.cells/htmlsaveoptions/sheetset/
---
## HtmlSaveOptions.SheetSet property

Получает или задает листы для рендеринга. По умолчанию — все видимые листы в книге: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Создать новую книгу с несколькими листами
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Сделать один лист скрытым для демонстрации
            workbook.Worksheets[1].IsVisible = false;

            // Установить некоторые примерные данные на каждом листе
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from {sheet.Name}");
            }

            // Создать экземпляр HtmlSaveOptions
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Отобразить текущее значение SheetSet (по умолчанию null, что означает все видимые листы)
            Console.WriteLine("Current SheetSet value: " + (options.SheetSet == null ? "All visible sheets" : "Custom set"));

            // Установить SheetSet так, чтобы включать только определённые листы (по индексу)
            options.SheetSet = new SheetSet(new int[] { 0, 2 });

            // Сохранить в HTML — будут включены только указанные листы
            workbook.Save("HtmlWithCustomSheetSet.html", options);

            // Изменить SheetSet, чтобы включать только видимые листы
            options.SheetSet = SheetSet.Visible;
            workbook.Save("HtmlWithVisibleSheets.html", options);

            // Изменить SheetSet, чтобы включать только активный лист
            workbook.Worksheets[2].IsSelected = true; // Activate the sheet by selecting it
            options.SheetSet = SheetSet.Active;
            workbook.Save("HtmlWithActiveSheet.html", options);
        }
    }
}
```

### См. также

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


