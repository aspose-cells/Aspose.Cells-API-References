---
title: "Cell.GetDisplayStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Возвращает стиль отображения этой ячейки"
type: docs
url: /ru/net/aspose.cells/cell/getdisplaystyle/
---
## GetDisplayStyle() {#getdisplaystyle}

Получает стиль отображения этой ячейки.

```csharp
public Style GetDisplayStyle()
```

### Возвращаемое значение

стиль отображения этой ячейки

### Примечания

То же, что использование SideBorders для `GetDisplayStyle`. То есть этот метод проверит и скорректирует верхние/нижние/левые/правые границы этой ячейки в соответствии со стилем([`GetStyle`](../getstyle/)) её соседних ячеек, но не будет проверять объединённые ячейки и не будет проверять стиль отображения соседних ячеек.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить стиль для ячейки A1
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = Color.FromArgb(157, 195, 230);
            worksheet.Cells["A1"].SetStyle(style1);
            
            // Установить стиль для ячейки A23
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = Color.Red;
            worksheet.Cells["A23"].SetStyle(style2);
            
            // Получить и отобразить стили
            Style displayStyle1 = worksheet.Cells["A1"].GetDisplayStyle();
            Console.WriteLine("A1 Foreground Color: " + displayStyle1.ForegroundColor);
            
            Style displayStyle2 = worksheet.Cells["A23"].GetDisplayStyle();
            Console.WriteLine("A23 Foreground Color: " + displayStyle2.ForegroundColor);
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

## GetDisplayStyle(bool) {#getdisplaystyle_2}

Получает стиль отображения этой ячейки.

```csharp
public Style GetDisplayStyle(bool includeMergedBorders)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| includeMergedBorders | Boolean | Указывает, проверять ли границы объединённых ячеек. |

### Возвращаемое значение

стиль отображения этой ячейки

### Примечания

Если указанный флаг равен false, то поведение такое же, как у `GetDisplayStyle`. В противном случае оно совпадает с использованием SideBorders&#x7C;DynamicStyleBorders для `GetDisplayStyle`.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Обратитесь к ячейке B2 и задайте некоторые свойства стиля
            Cell cell = worksheet.Cells["B2"];
            Style cellStyle = cell.GetStyle();
            cellStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            cell.SetStyle(cellStyle);
            
            // Получить стиль отображения с форматированием (параметр true)
            Style displayStyle = cell.GetDisplayStyle(true);
            
            // Вывести стиль линии правой границы
            Console.WriteLine("Right Border Line Style: " + displayStyle.Borders[BorderType.RightBorder].LineStyle);
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

## GetDisplayStyle(BorderType) {#getdisplaystyle_1}

Получает стиль отображения этой ячейки.

```csharp
public Style GetDisplayStyle(BorderType adjacentBorders)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| adjacentBorders | BorderType | Указывает, какие границы необходимо проверять и корректировать в соответствии с границами соседних ячеек. |

### Возвращаемое значение

стиль отображения этой ячейки

### Примечания

Если на эту ячейку также влияют другие настройки, такие как условное форматирование, объекты списка и т.д., то стиль отображения может отличаться от [`GetStyle`](../getstyle/). Для флагов, регулирующих границы в соответствии с соседними ячейками, TopBorder/BottomBorder/LeftBorder/RightBorder обозначают, следует ли проверять и объединять нижнюю/верхнюю/правую/левую границы соответствующих соседних ячеек слева/справа/сверху/снизу от текущей. С учётом производительности и совместимости некоторые перечисления используются для обозначения специальных операций: Horizontal/Vertical указывают, следует ли проверять и объединять нижнюю/правую границу объединённых ячеек с текущей. Diagonal (то есть одновременно установлены DiagonalUpBorder и DiagonalDownBorder) обозначает проверку и объединение границ из стиля отображения соседних ячеек. Обратите внимание, что проверка границ/стилей соседних ячеек, особенно стилей отображения, является затратным по времени процессом. Если нет необходимости получать границы для возвращаемого стиля, использование None для отключения обработки соседних ячеек улучшит производительность. При получении границ соседних ячеек из стилей, определённых только в этих ячейках (без установки Diagonal), производительность также может быть лучше, поскольку проверка стиля отображения одной ячейки тоже затратна.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBorderTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Установить примерные данные
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Создайте условное форматирование
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 9, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Получить стиль отображения с различными типами границ
            for (int i = 0; i < 10; i++)
            {
                Style styleWithBorder = cells[i, 0].GetDisplayStyle(BorderType.TopBorder);
                Style styleWithoutBorder = cells[i, 0].GetDisplayStyle(BorderType.None);

                Console.WriteLine($"Cell {i + 1}:");
                Console.WriteLine($"  Style with border - Foreground: {styleWithBorder.ForegroundArgbColor:X}");
                Console.WriteLine($"  Style without border - Foreground: {styleWithoutBorder.ForegroundArgbColor:X}");
            }
        }
    }
}
```

### См. также

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


