---
title: "VbaProjectReference.ExtendedLibid"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство VbaProjectReference. Получает и задает расширенный Libid ссылки"
type: docs
url: /ru/net/aspose.cells.vba/vbaprojectreference/extendedlibid/
---
## VbaProjectReference.ExtendedLibid property

Получает и задает расширенный Libid ссылки.

```csharp
public string ExtendedLibid { get; set; }
```

### Примечания

Только для ссылки на элемент управления.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaProjectReferencePropertyExtendedLibidDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Инициализировать проект VBA
                VbaProject vbaProject = workbook.VbaProject;

                // Добавить ссылку на элемент управления для демонстрации ExtendedLibid
                vbaProject.References.AddControlRefrernce(
                    "SampleControl",
                    "{00020430-0000-0000-C000-000000000046}",
                    "stdole2.tlb",
                    "2.0");

                // Получить первую ссылку
                VbaProjectReference reference = vbaProject.References[0];

                // Отобразить значение свойства ExtendedLibid
                Console.WriteLine("ExtendedLibid value: " + reference.ExtendedLibid);

                // Продемонстрировать установку ExtendedLibid (поскольку он доступен для чтения/записи)
                reference.ExtendedLibid = "3.0";
                Console.WriteLine("Updated ExtendedLibid value: " + reference.ExtendedLibid);

                // Сохраните книгу
                workbook.Save("ExtendedLibidDemo.xlsm");
                Console.WriteLine("Workbook saved successfully with ExtendedLibid demonstration.");
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

* class [VbaProjectReference](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


