---
title: "GridSheetRender.ToImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GridSheetRender metod. Renderar en viss sida till en Graphics"
type: docs
url: /sv/net/aspose.cells.griddesktop.data/gridsheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Rendera en viss sida till en Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |
| g | Graphics | Objektet att rendera till. |
| x | Single | X‑koordinaten (i pixlar) för det övre vänstra hörnet av den renderade sidan. |
| y | Single | Y‑koordinaten (i pixlar) för det övre vänstra hörnet av den renderade sidan. |
| bredd | Single | Den maximala bredden (i pixlar) som den renderade sidan kan uppta. |
| höjd | Single | Den maximala höjden (i pixlar) som den renderade sidan kan uppta. |

### Se även

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Rendera en viss sida till en Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |
| g | Graphics | Objektet att rendera till. |
| x | Single | X‑koordinaten (i pixlar) för det övre vänstra hörnet av den renderade sidan. |
| y | Single | Y‑koordinaten (i pixlar) för det övre vänstra hörnet av den renderade sidan. |

### Se även

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, string) {#toimage_4}

Rendera en viss sida till en fil.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |
| fileName | String | filnamn för den utgående bilden |

### Exempel

Följande kod skriver ut den första sidan av det första bladet till en png‑bild.

```csharp
//läs in källfilen med bilder.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//ange output‑bildtyp.
imgOpt.ImageType = ImageType.Png;

//rendera det första bladet.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//skriv ut den första sidan av bladet till en bild.
sr.ToImage(0, "output.png");
```

### Se även

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Stream) {#toimage_3}

Rendera en viss sida till en ström.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |
| ström | Ström | strömmen för den utgående bilden |

### Se även

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int) {#toimage}

Rendera en viss sida till ett Bitmap-objekt.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |

### Returvärde

bitmap-objektet för sidan

### Se även

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


