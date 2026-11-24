---
title: "GridSheetRender.ToImage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GridSheetRender method. Rendert eine bestimmte Seite zu einem Graphics‑Objekt."
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridsheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Bestimmte Seite in ein Graphics-Objekt rendern

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Seitenindex | Int32 | Geben Sie an, welche Seite konvertiert werden soll |
| g | Graphics | Das Objekt, in das gerendert werden soll. |
| x | Einzeln | Die X‑Koordinate (in Pixeln) der oberen linken Ecke der gerenderten Seite. |
| y | Einzeln | Die Y‑Koordinate (in Pixeln) der oberen linken Ecke der gerenderten Seite. |
| Breite | Einzeln | Die maximale Breite (in Pixeln), die die gerenderte Seite einnehmen kann. |
| Höhe | Einzeln | Die maximale Höhe (in Pixeln), die die gerenderte Seite einnehmen kann. |

### Siehe auch

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Bestimmte Seite in ein Graphics-Objekt rendern

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Seitenindex | Int32 | Geben Sie an, welche Seite konvertiert werden soll |
| g | Graphics | Das Objekt, in das gerendert werden soll. |
| x | Einzeln | Die X‑Koordinate (in Pixeln) der oberen linken Ecke der gerenderten Seite. |
| y | Einzeln | Die Y‑Koordinate (in Pixeln) der oberen linken Ecke der gerenderten Seite. |

### Siehe auch

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, string) {#toimage_4}

Rendert eine bestimmte Seite in eine Datei.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Seitenindex | Int32 | Geben Sie an, welche Seite konvertiert werden soll |
| fileName | String | Dateiname des Ausgabebildes |

### Beispiele

Der folgende Code gibt die erste Seite des ersten Blatts als PNG‑Bild aus.

```csharp
//Laden Sie die Quelldatei mit Bildern.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//Ausgabetyp des Bildes festlegen.
imgOpt.ImageType = ImageType.Png;

//Das erste Blatt rendern.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//Die erste Seite des Blatts als Bild ausgeben.
sr.ToImage(0, "output.png");
```

### Siehe auch

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Stream) {#toimage_3}

Rendert eine bestimmte Seite in einen Stream.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Seitenindex | Int32 | Geben Sie an, welche Seite konvertiert werden soll |
| Stream | Stream | der Stream des Ausgabebildes |

### Siehe auch

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int) {#toimage}

Rendert eine bestimmte Seite in ein Bitmap-Objekt.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Seitenindex | Int32 | Geben Sie an, welche Seite konvertiert werden soll |

### Rückgabewert

das Bitmap-Objekt der Seite

### Siehe auch

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


