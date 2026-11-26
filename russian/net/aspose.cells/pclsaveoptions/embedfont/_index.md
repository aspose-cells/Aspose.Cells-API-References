---
title: "PclSaveOptions.EmbedFont"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PclSaveOptions. Указывает, следует ли внедрять шрифт в выходной файл Pcl"
type: docs
url: /ru/net/aspose.cells/pclsaveoptions/embedfont/
---
## PclSaveOptions.EmbedFont property

Указывает, следует ли встраивать шрифт в выходной файл Pcl.

```csharp
public bool EmbedFont { get; set; }
```

### Примечания

Значение по умолчанию — true.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsPropertyEmbedFontDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и добавьте несколько примерных данных
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demonstrating EmbedFont property");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            try
            {
                // Создать параметры сохранения PCL.
                PclSaveOptions pclOptions = new PclSaveOptions();

                // Прочитайте и отобразите текущее значение свойства EmbedFont
                Console.WriteLine("Current EmbedFont value: " + pclOptions.EmbedFont);

                // (Опционально) Если свойство доступно для записи, вы можете установить его, но здесь мы только читаем его
                // pclOptions.EmbedFont = true;

                // Сохраните книгу в файл PCL, используя параметры
                workbook.Save("EmbedFontDemo.pcl", pclOptions);

                Console.WriteLine("Workbook saved successfully with EmbedFont demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


