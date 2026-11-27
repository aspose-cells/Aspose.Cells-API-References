---
title: "TableStyleElementCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TableStyleElementCollection-egenskap. Hämtar ett element av tabellstilen med indexet"
type: docs
url: /sv/net/aspose.cells.tables/tablestyleelementcollection/item/
---
## TableStyleElementCollection indexer (1 of 2)

Hämtar ett element av tabellstilen med indexet.

```csharp
public TableStyleElement this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet. |

### Returvärde

Returnerar [`TableStyleElement`](../../tablestyleelement/) objekt

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleElementCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Style firstColStyle = workbook.CreateStyle();
            firstColStyle.Pattern = BackgroundType.Solid;
            firstColStyle.BackgroundColor = System.Drawing.Color.LightBlue;

            string styleName = "CustomTableStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            TableStyleElementCollection elements = tableStyle.TableStyleElements;
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);
            TableStyleElement element = elements[elementIndex];
            element.SetElementStyle(firstColStyle);

            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data");

            int tableIndex = workbook.Worksheets[0].ListObjects.Add(0, 0, 1, 0, true);
            ListObject table = workbook.Worksheets[0].ListObjects[tableIndex];
            table.ShowTableStyleFirstColumn = true;
            table.TableStyleName = styleName;

            workbook.Save("TableStyleElementDemo.xlsx");
        }
    }
}
```

### Se även

* class [TableStyleElement](../../tablestyleelement/)
* class [TableStyleElementCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## TableStyleElementCollection indexer (2 of 2)

Hämtar elementet i tabellstilen efter elementtypen.

```csharp
public TableStyleElement this[TableStyleElementType type] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| typ | Elementtypen. |

### Returvärde

Returnerar [`TableStyleElement`](../../tablestyleelement/) objekt

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa en anpassad tabellstil
            string styleName = "CustomTableStyle";
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            int styleIndex = tableStyles.AddTableStyle(styleName);
            TableStyle tableStyle = tableStyles[styleIndex];

            // Kom åt TableStyleElementCollection
            TableStyleElementCollection elements = tableStyle.TableStyleElements;

            // Lägg till ett tabellstilelement
            int elementIndex = elements.Add(TableStyleElementType.FirstColumn);

            try
            {
                // Kom åt Item-egenskapen med indexeraren (som använder Item-egenskapen internt)
                TableStyleElement element = elements[elementIndex];

                // Visa information om elementet
                Console.WriteLine("Table Style Element Type: " + element.Type);
                Console.WriteLine("Element has been successfully accessed via Item property");

                // Spara arbetsboken
                workbook.Save("TableStyleElementItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [TableStyleElement](../../tablestyleelement/)
* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElementCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


