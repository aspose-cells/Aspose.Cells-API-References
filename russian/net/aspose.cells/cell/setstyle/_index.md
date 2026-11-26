---
title: "Cell.SetStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Устанавливает стиль ячейки"
type: docs
url: /ru/net/aspose.cells/cell/setstyle/
---
## SetStyle(Style) {#setstyle}

Устанавливает стиль ячейки.

```csharp
public void SetStyle(Style style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | Стиль ячейки. |

### Примечания

Если настройки границы изменены, граница корректируемых ячеек также будет обновлена.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создайте стиль и задайте его свойства
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;

            // Примените стиль к ячейке B2 (1,1 в индексе, начинающемся с нуля)
            cells[1, 1].SetStyle(style);

            // Сохраните книгу
            workbook.Save("SetStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, bool) {#setstyle_2}

Применяет изменённое свойство стиля к ячейке.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | Стиль ячейки. |
| explicitFlag | Boolean | True, только перезаписывая форматирование, которое явно задано. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создавайте стили напрямую
            Style style1 = workbook.CreateStyle();
            style1.Name = "MyStyle1";
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.Font.IsBold = true;
            
            Style style2 = workbook.CreateStyle();
            style2.Name = "MyStyle2";
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            style2.Font.Color = System.Drawing.Color.Red;
            
            // Применяйте стили к ячейкам с помощью метода SetStyle
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("Styled Text 1");
            cell1.SetStyle(style1, true); // true to preserve existing style elements not defined in the new style
            
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Styled Text 2");
            cell2.SetStyle(style2, false); // false to overwrite all style elements
            
            // Сохраните книгу
            workbook.Save("SetStyleDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, StyleFlag) {#setstyle_1}

Применить стиль ячейки на основе флагов.

```csharp
public void SetStyle(Style style, StyleFlag flag)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| стиль | Стиль | Стиль ячейки. |
| флаг | StyleFlag | Флаг стиля. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создайте стиль и задайте его свойства
            Style style = workbook.CreateStyle();
            style.Font.Color = Color.Red;
            style.Name = "CustomStyle";

            // Создайте флаг стиля и установите его для применения всего форматирования
            StyleFlag flag = new StyleFlag();
            flag.All = true;

            // Получите ячейки и задайте значение A1
            Cells cells = sheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");

            // Примените стиль к ячейке, используя SetStyle
            cell.SetStyle(style, flag);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


