---
title: "WorkbookDesigner.GetSmartMarkers"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorkbookDesigner. Возвращает коллекцию умных маркеров в электронной таблице"
type: docs
url: /ru/net/aspose.cells/workbookdesigner/getsmartmarkers/
---
## WorkbookDesigner.GetSmartMarkers method

Возвращает коллекцию смарт‑маркировок в электронной таблице.

```csharp
public string[] GetSmartMarkers()
```

### Возвращаемое значение

Коллекция умных маркеров

### Примечания

Массив строк создаётся при каждом вызове. Массив сортируется, а дублирующие значения удаляются.

### Примеры

```csharp
using System;
using System.Data;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodGetSmartMarkersDemo
    {
        public static void Run()
        {
            // Создать пример файла шаблона в памяти
            Workbook templateWorkbook = new Workbook();
            Cells cells = templateWorkbook.Worksheets[0].Cells;
            
            // Добавить умные маркеры в шаблон
            cells["A1"].PutValue("&=COLORS_TIMES.COLORS");
            cells["B1"].PutValue("&=COLORS_TIMES.TIMES");
            
            // Сохранить шаблон в поток памяти
            MemoryStream templateStream = new MemoryStream();
            templateWorkbook.Save(templateStream, SaveFormat.Xlsx);
            
            // Инициализировать WorkbookDesigner с шаблоном
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook(templateStream);
            
            // Получить и отобразить смарт‑маркировки
            string[] smartMarkers = designer.GetSmartMarkers();
            Console.WriteLine("Found smart markers:");
            foreach (string marker in smartMarkers)
            {
                Console.WriteLine(marker);
            }
            
            // Подготовьте источник данных
            DataTable data = new DataTable("COLORS_TIMES");
            data.Columns.Add("COLORS", typeof(string));
            data.Columns.Add("TIMES", typeof(DateTime));
            data.Rows.Add("red", DateTime.Now.AddDays(-1));
            data.Rows.Add("yellow", DateTime.Now);
            data.Rows.Add("green", DateTime.Now.AddDays(1));
            
            // Установите источник данных и выполните обработку
            designer.SetDataSource(data);
            designer.Process();
            
            // Сохранить результат
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


