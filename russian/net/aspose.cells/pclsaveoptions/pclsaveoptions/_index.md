---
title: "PclSaveOptions.PclSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор PclSaveOptions. Создает параметры для сохранения файла pcl"
type: docs
url: /ru/net/aspose.cells/pclsaveoptions/pclsaveoptions/
---
## PclSaveOptions constructor

Создает параметры для сохранения файла pcl.

```csharp
public PclSaveOptions()
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить некоторые образцы данных в лист
            worksheet.Cells["A1"].PutValue("PCL Save Options Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates PclSaveOptions constructor");
            
            try
            {
                // Вызовите метод #ctor для создания экземпляра PclSaveOptions
                PclSaveOptions pclOptions = new PclSaveOptions();
                
                // Настройте дополнительные параметры при необходимости
                pclOptions.AddPrinterFont("Arial", "ArialPCL");
                
                Console.WriteLine("PclSaveOptions created successfully");
                
                // Сохраните книгу с параметрами PCL
                workbook.Save("PclSaveOptionsDemo.pcl", pclOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating PclSaveOptions: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


