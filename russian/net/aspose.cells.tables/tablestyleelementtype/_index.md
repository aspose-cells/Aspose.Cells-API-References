---
title: "Перечисление TableStyleElementType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Tables.TableStyleElementType. Представляет тип элемента стиля таблицы или сводной таблицы."
type: docs
url: /ru/net/aspose.cells.tables/tablestyleelementtype/
---
## TableStyleElementType enumeration

Представляет тип элемента стиля таблицы или сводной таблицы.

```csharp
public enum TableStyleElementType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| BlankRow | `18` | Элемент стиля таблицы, применяемый к пустым строкам сводной таблицы. |
| FirstColumn | `8` | Элемент стиля таблицы, применяемый к первому столбцу таблицы. |
| FirstColumnStripe | `3` | Элемент стиля таблицы, применяемый к полосам первого столбца таблицы. |
| FirstColumnSubheading | `22` | Элемент стиля таблицы, применяемый к подзаголовку первого столбца сводной таблицы. |
| FirstHeaderCell | `11` | Элемент стиля таблицы, применяемый к ячейке первой строки заголовка таблицы. |
| FirstRowStripe | `5` | Элемент стиля таблицы, применяемый к полосам первой строки таблицы. |
| FirstRowSubheading | `25` | Элемент стиля таблицы, применяемый к подзаголовку первой строки сводной таблицы. |
| FirstSubtotalColumn | `15` | Элемент стиля таблицы, применяемый к первому столбцу промежуточного итога сводной таблицы. |
| FirstSubtotalRow | `19` | Элемент стиля таблицы, применяемый к первой строке промежуточного итога сводной таблицы. |
| GrandTotalColumn | `28` | Элемент стиля таблицы, применяемый к столбцу итоговой суммы сводной таблицы. |
| GrandTotalRow | `29` | Элемент стиля таблицы, применяемый к строке итоговой суммы сводной таблицы. |
| FirstTotalCell | `13` | Элемент стиля таблицы, применяемый к ячейке первой строки итогов таблицы. |
| HeaderRow | `9` | Элемент стиля таблицы, применяемый к строке заголовка таблицы. |
| LastColumn | `7` | Элемент стиля таблицы, применяемый к последнему столбцу таблицы. |
| LastHeaderCell | `12` | Элемент стиля таблицы, применяемый к ячейке последней строки заголовка таблицы. |
| LastTotalCell | `14` | Элемент стиля таблицы, применяемый к ячейке последней строки итогов таблицы. |
| PageFieldLabels | `1` | Элемент стиля таблицы, применяемый к меткам полей страниц сводной таблицы. |
| PageFieldValues | `2` | Элемент стиля таблицы, применяемый к значениям полей страниц сводной таблицы. |
| SecondColumnStripe | `4` | Элемент стиля таблицы, применяемый к полосам второй колонки таблицы. |
| SecondColumnSubheading | `23` | Элемент стиля таблицы, применяемый к подзаголовку второй колонки сводной таблицы. |
| SecondRowStripe | `6` | Элемент стиля таблицы, применяемый к полосам второй строки таблицы. |
| SecondRowSubheading | `26` | Элемент стиля таблицы, применяемый к подзаголовку второй строки сводной таблицы. |
| SecondSubtotalColumn | `16` | Элемент стиля таблицы, применяемый к второй колонке подытога сводной таблицы. |
| SecondSubtotalRow | `20` | Элемент стиля таблицы, применяемый ко второй строке подытога сводной таблицы. |
| ThirdColumnSubheading | `24` | Элемент стиля таблицы, применяемый к подзаголовку третьей колонки сводной таблицы. |
| ThirdRowSubheading | `27` | Элемент стиля таблицы, применяемый к подзаголовку третьей строки сводной таблицы. |
| ThirdSubtotalColumn | `17` | Элемент стиля таблицы, применяемый к третьей колонке подытога сводной таблицы. |
| ThirdSubtotalRow | `21` | Элемент стиля таблицы, применяемый к третьей строке подытога сводной таблицы. |
| TotalRow | `10` | Элемент стиля таблицы, применяемый к строке итогов таблицы. |
| WholeTable | `0` | Элемент стиля таблицы, применяемый ко всему содержимому таблицы. |
| LastColumnSubheading | `130` | Элемент стиля таблицы, применяемый к полю последней колонки сводной таблицы. |
| LastRowSubheading | `131` | Элемент стиля таблицы, применяемый к полю последней строки сводной таблицы. |
| LastSubtotalRow | `133` | Элемент стиля таблицы, применяемый к полю последней строки подытога сводной таблицы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TablesClassTableStyleElementTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Style firstColumnStyle = workbook.CreateStyle();
            firstColumnStyle.Pattern = BackgroundType.Solid;
            firstColumnStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            
            Style lastColumnStyle = workbook.CreateStyle();
            lastColumnStyle.Font.IsBold = true;
            lastColumnStyle.Pattern = BackgroundType.Solid;
            lastColumnStyle.ForegroundColor = System.Drawing.Color.LightGreen;

            string tableStyleName = "CustomStyle1";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(tableStyleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            TableStyleElementCollection elements = tableStyle.TableStyleElements;
            
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);
            elements[elementIndex].SetElementStyle(firstColumnStyle);
            
            elementIndex = elements.Add(TableStyleElementType.LastColumn);
            elements[elementIndex].SetElementStyle(lastColumnStyle);

            Cells cells = workbook.Worksheets[0].Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue($"Column {i + 1}");
            }

            for (int row = 1; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue(row * col);
                }
            }

            ListObject table = workbook.Worksheets[0].ListObjects[workbook.Worksheets[0].ListObjects.Add(0, 0, 4, 4, true)];
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.TableStyleName = tableStyleName;

            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


