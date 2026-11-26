---
title: "AbstractTextLoadOptions.LoadStyleStrategy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AbstractTextLoadOptions. Указывает стратегию применения стиля к разобранным значениям при преобразовании строкового значения в число или дату/время"
type: docs
url: /ru/net/aspose.cells/abstracttextloadoptions/loadstylestrategy/
---
## AbstractTextLoadOptions.LoadStyleStrategy property

Указывает стратегию применения стиля к разобранным значениям при преобразовании строкового значения в число или дату/время.

```csharp
public TxtLoadStyleStrategy LoadStyleStrategy { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyLoadStyleStrategyDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите пользовательский стиль для демонстрации
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.Name = "Arial";
            customStyle.Font.Size = 12;
            customStyle.Font.Color = System.Drawing.Color.Blue;
            customStyle.Pattern = BackgroundType.Solid;
            customStyle.ForegroundColor = System.Drawing.Color.LightYellow;

            // Применить стиль к ячейке
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");
            cell.SetStyle(customStyle);

            // Создайте CSV‑данные
            string csvData = "Data1,Data2\nValue1,Value2";
            byte[] byteArray = Encoding.ASCII.GetBytes(csvData);
            MemoryStream stream = new MemoryStream(byteArray);

            // Создайте параметры загрузки текста с LoadStyleStrategy
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn
            };

            // Импортируйте CSV‑данные с указанными параметрами загрузки
            cells.ImportCSV(stream, loadOptions, 0, 0);

            // Сохранить книгу, чтобы продемонстрировать результат
            workbook.Save("LoadStyleStrategyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [TxtLoadStyleStrategy](../../txtloadstylestrategy/)
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


