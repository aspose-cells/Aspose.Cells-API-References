---
title: "HyperlinkCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HyperlinkCollection-Methode. Fügt einem angegebenen Zellbereich oder einer einzelnen Zelle einen Hyperlink hinzu"
type: docs
url: /de/net/aspose.cells/hyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstRow | Int32 | Erste Zeile des Hyperlink-Bereichs. |
| firstColumn | Int32 | Erste Spalte des Hyperlink-Bereichs. |
| totalRows | Int32 | Anzahl der Zeilen in diesem Hyperlink-Bereich. |
| totalColumns | Int32 | Anzahl der Spalten dieses Hyperlink-Bereichs. |
| address | String | Adresse des Hyperlinks. |

### Rückgabewert

[`Hyperlink`](../../hyperlink/) object index.

### Beispiele

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

            // Hyperlink hinzufügen unter Verwendung von Zeilen-/Spaltenkoordinaten und Abmessungen
            worksheet.Hyperlinks.Add(0, 0, 1, 1, "http://www.aspose.com");
            worksheet.Hyperlinks.Add(1, 0, 1, 1, "c:\\book1.xls");
            
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_1}

Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Zellname. |
| totalRows | Int32 | Anzahl der Zeilen in diesem Hyperlink-Bereich. |
| totalColumns | Int32 | Anzahl der Spalten dieses Hyperlink-Bereichs. |
| address | String | Adresse des Hyperlinks. |

### Rückgabewert

[`Hyperlink`](../../hyperlink/) object index.

### Beispiele

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

            // Hyperlink zu Zelle A1 mit Adresse "www.aspose.com" hinzufügen
            hyperlinks.Add("A1", 1, 1, "www.aspose.com");
            
            // Hyperlink-Adresse anzeigen
            Console.WriteLine("Hyperlink Address: " + worksheet.Cells["A1"].StringValue);
            
            // Anzeigetext ändern
            worksheet.Cells["A1"].PutValue("Click Here");
            Console.WriteLine("Display Text: " + hyperlinks[0].TextToDisplay);
            
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, string, string) {#add_2}

Fügt einen Hyperlink zu einer angegebenen Zelle oder einem Zellbereich hinzu.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startCellName | String | Die Zelle oben links des Bereichs. |
| endCellName | String | Die Zelle unten rechts des Bereichs. |
| address | String | Adresse des Hyperlinks. |
| textToDisplay | String | Der Text, der für den angegebenen Hyperlink angezeigt werden soll. |
| screenTip | String | Der ScreenTip-Text für den angegebenen Hyperlink. |

### Rückgabewert

[`Hyperlink`](../../hyperlink/) object index.

### Beispiele

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

            // Demonstration der Add-Methode mit (String, String, String, String, String)-Parametern
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            workbook.Save("HyperlinkCollectionExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


