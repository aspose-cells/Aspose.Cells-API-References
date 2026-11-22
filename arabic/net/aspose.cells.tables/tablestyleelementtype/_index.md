---
title: "Enum TableStyleElementType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Tables.TableStyleElementType enum. يمثل نوع عنصر نمط الجدول أو PivotTable"
type: docs
url: /ar/net/aspose.cells.tables/tablestyleelementtype/
---
## TableStyleElementType enumeration

يمثل نوع عنصر نمط الجدول أو PivotTable.

```csharp
public enum TableStyleElementType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| BlankRow | `18` | عنصر نمط الجدول الذي يُطبق على صفوف PivotTable الفارغة. |
| FirstColumn | `8` | عنصر نمط الجدول الذي يُطبق على العمود الأول للجدول. |
| FirstColumnStripe | `3` | عنصر نمط الجدول الذي يُطبق على خطوط العمود الأول للجدول. |
| FirstColumnSubheading | `22` | عنصر نمط الجدول الذي يُطبق على العنوان الفرعي للعمود الأول في PivotTable. |
| FirstHeaderCell | `11` | عنصر نمط الجدول الذي يُطبق على خلية الصف الأول في رأس الجدول. |
| FirstRowStripe | `5` | عنصر نمط الجدول الذي يُطبق على خطوط الصف الأول للجدول. |
| FirstRowSubheading | `25` | عنصر نمط الجدول الذي يُطبق على العنوان الفرعي للصف الأول في PivotTable. |
| FirstSubtotalColumn | `15` | عنصر نمط الجدول الذي يُطبق على العمود الأول للملخص الفرعي في PivotTable. |
| FirstSubtotalRow | `19` | عنصر نمط الجدول الذي يُطبق على الصف الأول للملخص الفرعي في pivot table. |
| GrandTotalColumn | `28` | عنصر نمط الجدول الذي يُطبق على عمود الإجمالي الكلي في pivot table. |
| GrandTotalRow | `29` | عنصر نمط الجدول الذي يُطبق على صف الإجمالي الكلي في pivot table. |
| FirstTotalCell | `13` | عنصر نمط الجدول الذي يُطبق على خلية الصف الأول الإجمالي في الجدول. |
| HeaderRow | `9` | عنصر نمط الجدول الذي يُطبق على صف رأس الجدول. |
| LastColumn | `7` | عنصر نمط الجدول الذي يُطبق على العمود الأخير للجدول. |
| LastHeaderCell | `12` | عنصر نمط الجدول الذي يُطبق على خلية الصف الأخير في رأس الجدول. |
| LastTotalCell | `14` | عنصر نمط الجدول الذي يُطبق على خلية الصف الأخير الإجمالي في الجدول. |
| PageFieldLabels | `1` | عنصر نمط الجدول الذي يُطبق على تسميات حقول الصفحة في pivot table. |
| PageFieldValues | `2` | عنصر نمط الجدول الذي يُطبق على قيم حقل الصفحة في جدول المحور. |
| SecondColumnStripe | `4` | عنصر نمط الجدول الذي يُطبق على خطوط العمود الثاني في الجدول. |
| SecondColumnSubheading | `23` | عنصر نمط الجدول الذي يُطبق على عنوان العمود الثاني في جدول المحور. |
| SecondRowStripe | `6` | عنصر نمط الجدول الذي يُطبق على خطوط الصف الثاني في الجدول. |
| SecondRowSubheading | `26` | عنصر نمط الجدول الذي يُطبق على عنوان الصف الثاني في جدول المحور. |
| SecondSubtotalColumn | `16` | عنصر نمط الجدول الذي يُطبق على العمود الفرعي الثاني في PivotTable. |
| SecondSubtotalRow | `20` | عنصر نمط الجدول الذي يُطبق على الصف الفرعي الثاني في PivotTable. |
| ThirdColumnSubheading | `24` | عنصر نمط الجدول الذي يُطبق على عنوان العمود الثالث في PivotTable. |
| ThirdRowSubheading | `27` | عنصر نمط الجدول الذي يُطبق على عنوان الصف الثالث في PivotTable. |
| ThirdSubtotalColumn | `17` | عنصر نمط الجدول الذي يُطبق على العمود الفرعي الثالث في جدول المحور. |
| ThirdSubtotalRow | `21` | عنصر نمط الجدول الذي يُطبق على الصف الفرعي الثالث في PivotTable. |
| TotalRow | `10` | عنصر نمط الجدول الذي يُطبق على الصف الإجمالي في الجدول. |
| WholeTable | `0` | عنصر نمط الجدول الذي يُطبق على المحتوى الكامل للجدول. |
| LastColumnSubheading | `130` | عنصر نمط الجدول الذي يُطبق على حقل العمود الأخير في جدول المحور. |
| LastRowSubheading | `131` | عنصر نمط الجدول الذي يُطبق على حقل الصف الأخير في جدول المحور. |
| LastSubtotalRow | `133` | عنصر نمط الجدول الذي يُطبق على حقل الصف الفرعي الأخير في جدول المحور. |

### أمثلة

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

### انظر أيضًا

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


