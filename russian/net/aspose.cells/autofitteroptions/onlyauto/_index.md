---
title: "AutoFitterOptions.OnlyAuto"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoFitterOptions. Указывает, следует ли подгонять только те строки, высота которых не задана вручную"
type: docs
url: /ru/net/aspose.cells/autofitteroptions/onlyauto/
---
## AutoFitterOptions.OnlyAuto property

Указывает, следует ли подгонять только те строки, высота которых не задана вручную.

```csharp
public bool OnlyAuto { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyOnlyAutoDemo
    {
        public static void Run()
        {
            // Создайте параметры загрузки и установите свойство OnlyAuto
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = new AutoFitterOptions();
            loadOptions.AutoFitterOptions.OnlyAuto = true;

            // Загрузите книгу с параметрами автоподгонки
            Workbook workbook = new Workbook("example.xml", loadOptions);
            
            // Продемонстрируйте автоподгонку, проверяя ширину столбца
            Console.WriteLine("Column width after auto-fit: " + 
                workbook.Worksheets[0].Cells.GetColumnWidthPixel(0));
            
            // Сохранить и перезагрузить, чтобы проверить сохранность
            workbook.Save("example_output.xlsx");
            Workbook reloaded = new Workbook("example_output.xlsx");
            Console.WriteLine("Reloaded column width: " + 
                reloaded.Worksheets[0].Cells.GetColumnWidthPixel(0));
        }
    }
}
```

### См. также

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


