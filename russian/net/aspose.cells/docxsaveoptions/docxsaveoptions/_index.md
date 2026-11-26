---
title: "DocxSaveOptions.DocxSaveOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор DocxSaveOptions. Представляет параметры сохранения файла .docx"
type: docs
url: /ru/net/aspose.cells/docxsaveoptions/docxsaveoptions/
---
## DocxSaveOptions() {#constructor}

Представляет параметры сохранения файла .docx.

```csharp
public DocxSaveOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к первому листу и добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Инициализируйте DocxSaveOptions с помощью конструктора
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.SaveAsEditableShaps = true;
            
            // Сохраните книгу в формате DOCX с параметрами
            workbook.Save("output.docx", saveOptions);
            
            Console.WriteLine("Document saved successfully with DocxSaveOptions.");
        }
    }
}
```

### См. также

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DocxSaveOptions(bool) {#constructor_1}

Представляет параметры сохранения файла .docx.

```csharp
public DocxSaveOptions(bool saveAsImage)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| saveAsImage | Boolean | Если True, рабочая книга будет преобразована в несколько изображений .docx файла. Если False, рабочая книга будет преобразована в несколько таблиц .docx файла. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Сохранить как DOCX с параметрами по умолчанию
            workbook.Save("output_default.docx");
            
            // Сохранить как DOCX с DocxSaveOptions(true) — оптимизировано для MS Word
            workbook.Save("output_optimized.docx", new DocxSaveOptions(true));
        }
    }
}
```

### См. также

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


