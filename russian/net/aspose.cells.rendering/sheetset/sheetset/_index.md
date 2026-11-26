---
title: "SheetSet.SheetSet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор SheetSet. Создаёт набор листов на основе точных индексов листов"
type: docs
url: /ru/net/aspose.cells.rendering/sheetset/sheetset/
---
## SheetSet(params int[]) {#constructor}

Создаёт набор листов на основе точных индексов листов.

```csharp
public SheetSet(params int[] sheetIndexes)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetIndexes | Int32[] | нумерация листов начинается с нуля. |

### Примечания

Если будет найден лист, отсутствующий в книге, во время рендеринга будет выброшено исключение.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithInt32ArrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу с 3 листами
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Добавьте идентификационный текст к каждому листу
            workbook.Worksheets[0].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets[1].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets[2].Cells["A1"].PutValue("This is Sheet 3");

            try
            {
                // Создайте SheetSet с конкретными индексами листов (0 и 2)
                SheetSet sheetSet = new SheetSet(new int[] { 0, 2 });

                // Создайте параметры сохранения PDF с нашим набором листов
                PdfSaveOptions options = new PdfSaveOptions();
                options.SheetSet = sheetSet;

                // Сохраните книгу с выбранными листами
                workbook.Save("SheetSetDemo.pdf", options);
                Console.WriteLine("Created PDF containing Sheet 1 and Sheet 3");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid sheet index specified: {ex.Message}");
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

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SheetSet(params string[]) {#constructor_1}

Создаёт набор листов на основе точных имён листов.

```csharp
public SheetSet(params string[] sheetNames)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sheetNames | String[] | имена листов. |

### Примечания

Если будет найден лист, отсутствующий в книге, во время рендеринга будет выброшено исключение.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetMethodCtorWithStringArrayDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и добавьте листы
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "First";
            workbook.Worksheets.Add("Second");
            workbook.Worksheets.Add("Third");

            workbook.Worksheets["First"].Cells["A1"].PutValue("This is Sheet 1");
            workbook.Worksheets["Second"].Cells["A1"].PutValue("This is Sheet 2");
            workbook.Worksheets["Third"].Cells["A1"].PutValue("This is Sheet 3");

            // Подготовьте имена листов для SheetSet
            string[] selectedSheets = { "First", "Third" };

            try
            {
                // Создайте SheetSet с параметром массив строк
                SheetSet sheetSet = new SheetSet(selectedSheets);

                // Настройте параметры сохранения PDF с созданным SheetSet
                PdfSaveOptions pdfOptions = new PdfSaveOptions();
                pdfOptions.SheetSet = sheetSet;

                // Сохраните книгу в PDF с указанными листами
                workbook.Save("SheetSetOutput.pdf", pdfOptions);

                Console.WriteLine("Created PDF with sheets: " + string.Join(", ", selectedSheets));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating SheetSet: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


