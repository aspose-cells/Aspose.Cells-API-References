---
title: "Workbook.CreateStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Создает новый стиль"
type: docs
url: /ru/net/aspose.cells/workbook/createstyle/
---
## CreateStyle() {#createstyle}

Создаёт новый стиль.

```csharp
public Style CreateStyle()
```

### Возвращаемое значение

Возвращает объект стиля.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать новый стиль с помощью метода CreateStyle
            Style newStyle = workbook.CreateStyle();
            
            // Установить свойства стиля
            newStyle.Font.Name = "Arial";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            newStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            newStyle.Pattern = BackgroundType.Solid;
            newStyle.IsTextWrapped = true;
            
            // Создать флаг стиля и установить флаги
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            flag.CellShading = true;
            flag.WrapText = true;
            
            // Применить стиль к ячейке A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text has a custom style with wrapping");
            worksheet.Cells.ApplyStyle(newStyle, flag);
            
            // Автоматически подогнать столбец
            worksheet.AutoFitColumn(0);
            
            // Сохраните книгу
            workbook.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateStyle(bool) {#createstyle_1}

Создаёт новый стиль.

```csharp
public Style CreateStyle(bool cloneDefaultStyle)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cloneDefaultStyle | Boolean | Указывает, клонирует ли стиль по умолчанию |

### Возвращаемое значение

Возвращает объект стиля.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook wb = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Создать новый стиль (false = не наследовать стиль по умолчанию)
            Style style = wb.CreateStyle(false);
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.IsBold = true;
            
            // Применить стиль к ячейке
            Cell cell = cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Styled Text");
            
            // Сохраните книгу
            wb.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


