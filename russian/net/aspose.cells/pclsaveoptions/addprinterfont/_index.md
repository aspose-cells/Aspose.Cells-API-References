---
title: "PclSaveOptions.AddPrinterFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PclSaveOptions. Добавляет информацию о шрифте, который уже добавлен в принтер производителем"
type: docs
url: /ru/net/aspose.cells/pclsaveoptions/addprinterfont/
---
## PclSaveOptions.AddPrinterFont method

Добавляет информацию о шрифте, который уже установлен в принтере производителем.

```csharp
public void AddPrinterFont(string fontFullName, string fontPclName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fontFullName | String | Полное название шрифта (например, "Times New Roman Bold Italic"), используемого в исходном файле. |
| fontPclName | String | Название шрифта, который будет использован в выходном документе Pcl. |

### Примечания

Согласно спецификации Pcl, в любом принтере должно быть встроено 52 шрифта. Однако производители могут добавить другие шрифты в свои устройства.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsMethodAddPrinterFontWithStringStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте немного текста в лист, чтобы продемонстрировать использование шрифта
            worksheet.Cells["A1"].PutValue("This text will use the added printer font");
            
            // Создать параметры сохранения PCL.
            PclSaveOptions pclSaveOptions = new PclSaveOptions();
            
            try
            {
                // Вызовите метод AddPrinterFont с конкретными названиями шрифтов
                pclSaveOptions.AddPrinterFont("Arial", "ArialPCL");
                pclSaveOptions.AddPrinterFont("Times New Roman", "TimesPCL");
                
                Console.WriteLine("AddPrinterFont method executed successfully with parameters (String, String)");
                
                // Сохраните книгу с параметрами PCL
                workbook.Save("PclWithAddedPrinterFonts.pcl", pclSaveOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddPrinterFont method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


