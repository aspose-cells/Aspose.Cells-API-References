---
title: "OoxmlSaveOptions.EmbedOoxmlAsOleObject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OoxmlSaveOptions. Указывает, следует ли встраивать файлы Ooxml объекта OleObject как ole‑объект"
type: docs
url: /ru/net/aspose.cells/ooxmlsaveoptions/embedooxmlasoleobject/
---
## OoxmlSaveOptions.EmbedOoxmlAsOleObject property

Указывает, встраиваются ли файлы Ooxml объекта OleObject как OLE‑объект.

```csharp
public bool EmbedOoxmlAsOleObject { get; set; }
```

### Примечания

Только для OleObject.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyEmbedOoxmlAsOleObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OLE Object Embedding");
            
            // Создайте параметры сохранения OOXML и установите EmbedOoxmlAsOleObject
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.EmbedOoxmlAsOleObject = true;
            
            // Сохраните книгу
            workbook.Save("output.xlsx", saveOptions);
            
            Console.WriteLine("Workbook saved with OOXML embedded as OLE object.");
        }
    }
}
```

### См. также

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


