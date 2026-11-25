---
title: "Enum TableStyleElementType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Tables.TableStyleElementType. Rappresenta il tipo di elemento di stile della Tabella o della Tabella Pivot."
type: docs
url: /it/net/aspose.cells.tables/tablestyleelementtype/
---
## TableStyleElementType enumeration

Rappresenta il tipo di elemento di stile della Tabella o della PivotTable.

```csharp
public enum TableStyleElementType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| BlankRow | `18` | Elemento di stile della tabella che si applica alle righe vuote della Tabella Pivot. |
| FirstColumn | `8` | Elemento di stile della tabella che si applica alla prima colonna della tabella. |
| FirstColumnStripe | `3` | Elemento di stile della tabella che si applica alle bande della prima colonna della tabella. |
| FirstColumnSubheading | `22` | Elemento di stile della tabella che si applica al sottotitolo della prima colonna della Tabella Pivot. |
| FirstHeaderCell | `11` | Elemento di stile della tabella che si applica alla prima cella della riga di intestazione della tabella. |
| FirstRowStripe | `5` | Elemento di stile della tabella che si applica alle bande della prima riga della tabella. |
| FirstRowSubheading | `25` | Elemento di stile della tabella che si applica al sottotitolo della prima riga della Tabella Pivot. |
| FirstSubtotalColumn | `15` | Elemento di stile della tabella che si applica alla prima colonna di subtotale della Tabella Pivot. |
| FirstSubtotalRow | `19` | Elemento di stile della tabella che si applica alla prima riga di subtotale della tabella pivot. |
| GrandTotalColumn | `28` | Elemento di stile della tabella che si applica alla colonna del totale generale della tabella pivot. |
| GrandTotalRow | `29` | Elemento di stile della tabella che si applica alla riga del totale generale della tabella pivot. |
| FirstTotalCell | `13` | Elemento di stile della tabella che si applica alla prima cella della riga del totale della tabella. |
| HeaderRow | `9` | Elemento di stile della tabella che si applica alla riga di intestazione della tabella. |
| LastColumn | `7` | Elemento di stile della tabella che si applica all'ultima colonna della tabella. |
| LastHeaderCell | `12` | Elemento di stile della tabella che si applica all'ultima cella della riga di intestazione della tabella. |
| LastTotalCell | `14` | Elemento di stile della tabella che si applica all'ultima cella della riga del totale della tabella. |
| PageFieldLabels | `1` | Elemento di stile della tabella che si applica alle etichette dei campi di pagina della tabella pivot. |
| PageFieldValues | `2` | Elemento di stile della tabella che si applica ai valori del campo pagina della tabella pivot. |
| SecondColumnStripe | `4` | Elemento di stile della tabella che si applica alle strisce della seconda colonna della tabella. |
| SecondColumnSubheading | `23` | Elemento di stile della tabella che si applica al sottotitolo della seconda colonna della tabella pivot. |
| SecondRowStripe | `6` | Elemento di stile della tabella che si applica alle strisce della seconda riga della tabella. |
| SecondRowSubheading | `26` | Elemento di stile della tabella che si applica al sottotitolo della seconda riga della tabella pivot. |
| SecondSubtotalColumn | `16` | Elemento di stile della tabella che si applica alla seconda colonna di subtotale della PivotTable. |
| SecondSubtotalRow | `20` | Elemento di stile della tabella che si applica alla seconda riga di subtotale della PivotTable. |
| ThirdColumnSubheading | `24` | Elemento di stile della tabella che si applica al sottotitolo della terza colonna della PivotTable. |
| ThirdRowSubheading | `27` | Elemento di stile della tabella che si applica al sottotitolo della terza riga della PivotTable. |
| ThirdSubtotalColumn | `17` | Elemento di stile della tabella che si applica alla terza colonna di subtotale della tabella pivot. |
| ThirdSubtotalRow | `21` | Elemento di stile della tabella che si applica alla terza riga di subtotale della PivotTable. |
| TotalRow | `10` | Elemento di stile della tabella che si applica alla riga totale della Tabella. |
| WholeTable | `0` | Elemento di stile della tabella che si applica all'intero contenuto della tabella. |
| LastColumnSubheading | `130` | Elemento di stile della tabella che si applica all'ultimo campo colonna della tabella pivot. |
| LastRowSubheading | `131` | Elemento di stile della tabella che si applica all'ultimo campo riga della tabella pivot. |
| LastSubtotalRow | `133` | Elemento di stile della tabella che si applica all'ultimo campo riga di subtotale della tabella pivot. |

### Esempi

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

### Vedi anche

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


