---
title: "Перечисление StyleModifyFlag"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.StyleModifyFlag. Флаги изменения стиля"
type: docs
url: /ru/net/aspose.cells/stylemodifyflag/
---
## StyleModifyFlag enumeration

Флаги изменения стиля.

```csharp
public enum StyleModifyFlag
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| LeftBorder | `256` | Указывает, изменена ли левая граница стиля. |
| RightBorder | `512` | Указывает, изменена ли правая граница стиля. |
| TopBorder | `1024` | Указывает, изменена ли верхняя граница стиля. |
| BottomBorder | `2048` | Указывает, изменена ли нижняя граница стиля. |
| DiagonalDownBorder | `4096` | Указывает, изменена ли диагональная граница (вниз) стиля. |
| DiagonalUpBorder | `8192` | Указывает, изменена ли диагональная граница (вверх) стиля. |
| HorizontalBorder | `32` | Указывает, изменена ли горизонтальная граница стиля. Только для динамического стиля, например условного форматирования. |
| VerticalBorder | `64` | Указывает, изменена ли вертикальная граница стиля. Только для динамического стиля, например условного форматирования. |
| SideBorders | `3840` | Указывает четыре боковые границы: LeftBorder, RightBorder, TopBorder и BottomBorder. |
| Diagonal | `12288` | Указывает диагональные границы: DiagonalDownBorder и DiagonalUpBorder. |
| DynamicStyleBorders | `96` | Указывает границы динамического стиля: HorizontalBorder и VerticalBorder. |
| Borders | `16224` | Указывает, изменена ли одна или несколько границ (LeftBorder, RightBorder, TopBorder, BottomBorder, Diagonal, HorizontalBorder, VerticalBorder) стиля. |
| NumberFormat | `16384` | Указывает, было ли изменено numberformat. |
| HorizontalAlignment | `32768` | Указывает, было ли изменено горизонтальное выравнивание. |
| VerticalAlignment | `65536` | Указывает, было ли изменено вертикальное выравнивание. |
| Indent | `131072` | Указывает, было ли изменено свойство indent. |
| Rotation | `262144` | Указывает, было ли изменено свойство rotation. |
| WrapText | `524288` | Указывает, было ли изменено свойство wrap text. |
| ShrinkToFit | `1048576` | Указывает, было ли изменено свойство shrink to fit. |
| TextDirection | `2097152` | Указывает, было ли изменено свойство text direction. |
| RelativeIndent | `128` | Указывает, было ли изменено свойство relative indent для стиля. Только для динамического стиля, такого как условное форматирование. |
| AlignmentSettings | `4161664` | Указывает, было ли изменено одно или несколько свойств, связанных с выравниванием (HorizontalAlignment, VerticalAlignment, Rotation, WrapText, WrapText, Indent, ShrinkToFit, TextDirection, RelativeIndent). |
| Pattern | `4194304` | Указывает, было ли изменено pattern затенения. |
| ForegroundColor | `8388608` | Указывает, был ли изменён цвет переднего плана. |
| BackgroundColor | `16777216` | Указывает, был ли изменён цвет фона. |
| CellShading | `29360128` | Указывает, было ли изменено одно или несколько свойств, связанных с затенением (Pattern, ForegroundColor, BackgroundColor). |
| Locked | `67108864` | Указывает, было ли изменено свойство locked. |
| HideFormula | `134217728` | Указывает, было ли изменено hide formula. |
| ProtectionSettings | `201326592` | Указывает, было ли изменено одно или несколько свойств, связанных с защитой (Locked, HideFormula). |
| FontSize | `1` | Указывает, был ли изменён размер шрифта. |
| FontName | `2` | Указывает, было ли изменено имя шрифта. |
| FontColor | `3` | Указывает, был ли изменён цвет шрифта. |
| FontWeight | `4` | Указывает, был ли изменён вес шрифта. |
| FontItalic | `5` | Указывает, было ли изменено свойство italic шрифта. |
| FontUnderline | `6` | Указывает, было ли изменено свойство underline шрифта. |
| FontStrike | `7` | Указывает, было ли изменено свойство strike шрифта. |
| FontScript | `8` | Указывает, было ли изменено свойство subscript или superscript шрифта. |
| FontFamily | `9` | Указывает, изменено ли семейство шрифтов. |
| FontCharset | `10` | Указывает, изменена ли кодировка шрифта. |
| FontScheme | `11` | не используется. |
| FontDirty | `12` | не используется. |
| FontSpellingError | `13` | не используется. |
| FontUFillTx | `14` | не используется. |
| FontSpacing | `15` | не используется. |
| FontKerning | `16` | не используется. |
| FontEqualize | `17` | не используется. |
| FontCap | `18` | не используется. |
| FontVerticalText | `19` |  |
| Font | `31` | Указывает, изменено ли одно или несколько свойств шрифта стиля. |
| All | `234881023` | Все свойства, которые можно изменить для стиля. |
| None | `0` | Свойство не указано. |

### Примечания

Комбинации нескольких свойств определены для удобства пользователя. При проверке, изменены ли они для одного стиля, возвращаемое значение указывает, изменено ли одно или несколько свойств в комбинации.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleModifyFlagDemo
    {
        public static void StyleModifyFlagExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить некоторые значения в листе
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A2"].PutValue(123.45);

            // Создать новый стиль
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Color = System.Drawing.Color.Blue;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;

            // Применить стиль к ячейке
            worksheet.Cells["A1"].SetStyle(style);

            // Проверить, какие свойства стиля были изменены
            bool isFontModified = style.IsModified(StyleModifyFlag.Font);
            bool isFontSizeModified = style.IsModified(StyleModifyFlag.FontSize);
            bool isFontColorModified = style.IsModified(StyleModifyFlag.FontColor);
            bool isHorizontalAlignmentModified = style.IsModified(StyleModifyFlag.HorizontalAlignment);

            // Выведите результаты
            Console.WriteLine("Font Modified: " + isFontModified);
            Console.WriteLine("Font Size Modified: " + isFontSizeModified);
            Console.WriteLine("Font Color Modified: " + isFontColorModified);
            Console.WriteLine("Horizontal Alignment Modified: " + isHorizontalAlignmentModified);

            // Сохраните книгу
            workbook.Save("StyleModifyFlagExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


