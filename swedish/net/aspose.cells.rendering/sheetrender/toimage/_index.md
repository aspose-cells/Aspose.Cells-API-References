---
title: ToImage
second_title: Aspose.Cells för .NET API-referens
description: Gör en viss sida till en Graphics
type: docs
weight: 60
url: /sv/net/aspose.cells.rendering/sheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Gör en viss sida till en Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |
| g | Graphics | Objektet där det ska renderas. |
| x | Single | X-koordinaten (i pixlar) i det övre vänstra hörnet på den renderade sidan. |
| y | Single | Y-koordinaten (i pixlar) i det övre vänstra hörnet på den renderade sidan. |
| width | Single | Den maximala bredd (i pixlar) som kan upptas av den renderade sidan. |
| height | Single | Den maximala höjden (i pixlar) som kan upptas av den renderade sidan. |

### Se även

* class [SheetRender](../../sheetrender)
* namnutrymme [Aspose.Cells.Rendering](../../sheetrender)
* hopsättning [Aspose.Cells](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Gör en viss sida till en Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |
| g | Graphics | Objektet där det ska renderas. |
| x | Single | X-koordinaten (i pixlar) i det övre vänstra hörnet på den renderade sidan. |
| y | Single | Y-koordinaten (i pixlar) i det övre vänstra hörnet på den renderade sidan. |

### Se även

* class [SheetRender](../../sheetrender)
* namnutrymme [Aspose.Cells.Rendering](../../sheetrender)
* hopsättning [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_4}

Gör en viss sida till en fil.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |
| fileName | String | filnamnet på utdatabilden |

### Exempel

Följande kod matar ut den första sidan av det första arket till png-bild.

```csharp
//ladda in källfilen med bilder.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//set ut bildtyp.
imgOpt.ImageType = ImageType.Png;

//rendera det första arket.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//mata ut den första sidan av arket till bild.
sr.ToImage(0, "output.png");
```

### Se även

* class [SheetRender](../../sheetrender)
* namnutrymme [Aspose.Cells.Rendering](../../sheetrender)
* hopsättning [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_3}

Gör en viss sida till en ström.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |
| stream | Stream | strömmen av utdatabilden |

### Se även

* class [SheetRender](../../sheetrender)
* namnutrymme [Aspose.Cells.Rendering](../../sheetrender)
* hopsättning [Aspose.Cells](../../../)

---

## ToImage(int) {#toimage}

Rendera en viss sida till ett bitmappsobjekt.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | ange vilken sida som ska konverteras |

### Returvärde

sidans bitmappsobjekt

### Se även

* class [SheetRender](../../sheetrender)
* namnutrymme [Aspose.Cells.Rendering](../../sheetrender)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
