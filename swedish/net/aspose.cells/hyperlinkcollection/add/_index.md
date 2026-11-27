---
title: "HyperlinkCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HyperlinkCollection-metod. Lägger till en hyperlänk i en angiven cell eller ett cellområde"
type: docs
url: /sv/net/aspose.cells/hyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Lägger till en hyperlänk till en angiven cell eller ett cellområde.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | Int32 | Första raden i hyperlänkområdet. |
| firstColumn | Int32 | Första kolumnen i hyperlänkområdet. |
| totalRows | Int32 | Antal rader i detta hyperlänksområde. |
| totalColumns | Int32 | Antal kolumner i detta hyperlänksområde. |
| adress | String | Adress för hyperlänken. |

### Returvärde

[`Hyperlink`](../../hyperlink/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till hyperlänk med rad-/kolumnkoordinater och dimensioner
            worksheet.Hyperlinks.Add(0, 0, 1, 1, "http://www.aspose.com");
            worksheet.Hyperlinks.Add(1, 0, 1, 1, "c:\\book1.xls");
            
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Se även

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_1}

Lägger till en hyperlänk till en angiven cell eller ett cellområde.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Cellnamn. |
| totalRows | Int32 | Antal rader i detta hyperlänksområde. |
| totalColumns | Int32 | Antal kolumner i detta hyperlänksområde. |
| adress | String | Adress för hyperlänken. |

### Returvärde

[`Hyperlink`](../../hyperlink/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Lägg till hyperlänk till cell A1 med adress "www.aspose.com"
            hyperlinks.Add("A1", 1, 1, "www.aspose.com");
            
            // Visa hyperlänkens adress
            Console.WriteLine("Hyperlink Address: " + worksheet.Cells["A1"].StringValue);
            
            // Ändra visningstexten
            worksheet.Cells["A1"].PutValue("Click Here");
            Console.WriteLine("Display Text: " + hyperlinks[0].TextToDisplay);
            
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### Se även

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, string, string) {#add_2}

Lägger till en hyperlänk till en angiven cell eller ett cellområde.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startCellName | String | Den övre vänstra cellen i området. |
| endCellName | String | Den nedre högra cellen i området. |
| adress | String | Adress för hyperlänken. |
| textToDisplay | String | Texten som ska visas för den angivna hyperlänken. |
| screenTip | String | ScreenTip-texten för den angivna hyperlänken. |

### Returvärde

[`Hyperlink`](../../hyperlink/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Demonstrera Add-metoden med (String, String, String, String, String)-parametrar
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            workbook.Save("HyperlinkCollectionExample.xlsx");
        }
    }
}
```

### Se även

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


