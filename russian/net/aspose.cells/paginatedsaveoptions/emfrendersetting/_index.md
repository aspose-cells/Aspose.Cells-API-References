---
title: "PaginatedSaveOptions.EmfRenderSetting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaginatedSaveOptions. Настройка для рендеринга метафайла Emf"
type: docs
url: /ru/net/aspose.cells/paginatedsaveoptions/emfrendersetting/
---
## PaginatedSaveOptions.EmfRenderSetting property

Настройка рендеринга метафайла Emf.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Примечания

EMF‑метафайлы, идентифицированные как "EMF+ Dual", могут содержать как записи EMF+, так и записи EMF. Любой тип записи может использоваться для рендеринга изображения, только записи EMF+, или только записи EMF. Когда установлен EmfPlusPrefer, записи EMF+ будут анализироваться при рендеринге страницы, в противном случае будут анализироваться только записи EMF. Значение по умолчанию — EmfOnly.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());

            // Создать изображение для демонстрации EMF
            worksheet.Pictures.Add(10, 10, "example.png");

            // Настроить параметры сохранения с настройками EMF, используя PdfSaveOptions
            PdfSaveOptions options = new PdfSaveOptions()
            {
                EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer
            };

            // Сохранить книгу с настройками EMF
            workbook.Save("EmfRenderSettingDemo.pdf", options);
        }
    }
}
```

### См. также

* enum [EmfRenderSetting](../../emfrendersetting/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


