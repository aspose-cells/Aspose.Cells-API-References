---
title: "WorkbookSettings.DiscardImageEditData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WorkbookSettings property. Указывает, следует ли отбрасывать данные редактирования изображения"
type: docs
url: /ru/net/aspose.cells/workbooksettings/discardimageeditdata/
---
## WorkbookSettings.DiscardImageEditData property

Указывает, отбрасывать ли редактируемые данные изображения.

```csharp
public bool DiscardImageEditData { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDiscardImageEditDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить изображение на лист
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // Установите DiscardImageEditData в true (по умолчанию false)
            workbook.Settings.DiscardImageEditData = true;
            
            // Сохраните книгу
            workbook.Save("output_with_discarded_image_data.xlsx", SaveFormat.Xlsx);
            
            // Проверьте, что настройка была применена
            Console.WriteLine("DiscardImageEditData is set to: " + workbook.Settings.DiscardImageEditData);
        }
    }
}
```

### См. также

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


