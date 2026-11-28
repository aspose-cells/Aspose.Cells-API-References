---
title: "Enum TableStyleElementType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Tables.TableStyleElementType enum. Tablo veya PivotTable stil öğesi türünü temsil eder."
type: docs
url: /tr/net/aspose.cells.tables/tablestyleelementtype/
---
## TableStyleElementType enumeration

Tablo veya PivotTable stil öğesi türünü temsil eder.

```csharp
public enum TableStyleElementType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| BlankRow | `18` | PivotTable'ın boş satırlarına uygulanan tablo stil öğesi. |
| FirstColumn | `8` | Tablonun ilk sütununa uygulanan tablo stil öğesi. |
| FirstColumnStripe | `3` | Tablonun ilk sütun şeritlerine uygulanan tablo stil öğesi. |
| FirstColumnSubheading | `22` | PivotTable'ın ilk sütun alt başlığına uygulanan tablo stil öğesi. |
| FirstHeaderCell | `11` | Tablonun ilk başlık satırı hücresine uygulanan tablo stil öğesi. |
| FirstRowStripe | `5` | Tablonun ilk satır şeritlerine uygulanan tablo stil öğesi. |
| FirstRowSubheading | `25` | PivotTable'ın ilk satır alt başlığına uygulanan tablo stil öğesi. |
| FirstSubtotalColumn | `15` | PivotTable'ın ilk ara toplam sütununa uygulanan tablo stil öğesi. |
| FirstSubtotalRow | `19` | Pivot tablo'nun ilk ara toplam satırına uygulanan tablo stil öğesi. |
| GrandTotalColumn | `28` | Pivot tablo'nun genel toplam sütununa uygulanan tablo stil öğesi. |
| GrandTotalRow | `29` | Pivot tablo'nun genel toplam satırına uygulanan tablo stil öğesi. |
| FirstTotalCell | `13` | Tablonun ilk toplam satır hücresine uygulanan tablo stil öğesi. |
| HeaderRow | `9` | Tablonun başlık satırına uygulanan tablo stil öğesi. |
| LastColumn | `7` | Tablonun son sütununa uygulanan tablo stil öğesi. |
| LastHeaderCell | `12` | Tablonun son başlık satırı hücresine uygulanan tablo stil öğesi. |
| LastTotalCell | `14` | Tablonun son toplam satır hücresine uygulanan tablo stil öğesi. |
| PageFieldLabels | `1` | Pivot tablo'nun sayfa alanı etiketlerine uygulanan tablo stil öğesi. |
| PageFieldValues | `2` | Özet tablonun sayfa alanı değerlerine uygulanan tablo stili öğesi. |
| SecondColumnStripe | `4` | Tablonun ikinci sütun çizgilerine uygulanan tablo stili öğesi. |
| SecondColumnSubheading | `23` | Özet tablonun ikinci sütun alt başlığına uygulanan tablo stili öğesi. |
| SecondRowStripe | `6` | Tablonun ikinci satır çizgilerine uygulanan tablo stili öğesi. |
| SecondRowSubheading | `26` | Özet tablonun ikinci satır alt başlığına uygulanan tablo stili öğesi. |
| SecondSubtotalColumn | `16` | PivotTable'ın ikinci alt toplam sütununa uygulanan tablo stili öğesi. |
| SecondSubtotalRow | `20` | PivotTable'ın ikinci alt toplam satırına uygulanan tablo stili öğesi. |
| ThirdColumnSubheading | `24` | PivotTable'ın üçüncü sütun alt başlığına uygulanan tablo stili öğesi. |
| ThirdRowSubheading | `27` | PivotTable'ın üçüncü satır alt başlığına uygulanan tablo stili öğesi. |
| ThirdSubtotalColumn | `17` | Özet tablonun üçüncü alt toplam sütununa uygulanan tablo stili öğesi. |
| ThirdSubtotalRow | `21` | PivotTable'ın üçüncü alt toplam satırına uygulanan tablo stili öğesi. |
| TotalRow | `10` | Tablonun toplam satırına uygulanan tablo stili öğesi. |
| WholeTable | `0` | Tablonun tüm içeriğine uygulanan tablo stili öğesi. |
| LastColumnSubheading | `130` | Özet tablonun son sütun alanına uygulanan tablo stili öğesi. |
| LastRowSubheading | `131` | Özet tablonun son satır alanına uygulanan tablo stili öğesi. |
| LastSubtotalRow | `133` | Özet tablonun son alt toplam satır alanına uygulanan tablo stili öğesi. |

### Örnekler

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

### Ayrıca Bakınız

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


