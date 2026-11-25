---
title: "GridSheetRender.ToImage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GridSheetRender. Renderizza una determinata pagina su un oggetto Graphics"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridsheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Renderizza una certa pagina su un oggetto Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | indica quale pagina deve essere convertita |
| g | Grafica | L'oggetto su cui eseguire il rendering. |
| x | Single | La coordinata X (in pixel) dell'angolo superiore sinistro della pagina renderizzata. |
| y | Single | La coordinata Y (in pixel) dell'angolo superiore sinistro della pagina renderizzata. |
| larghezza | Single | La larghezza massima (in pixel) che può occupare la pagina renderizzata. |
| altezza | Single | L'altezza massima (in pixel) che può occupare la pagina renderizzata. |

### Vedi anche

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Renderizza una certa pagina su un oggetto Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | indica quale pagina deve essere convertita |
| g | Grafica | L'oggetto su cui eseguire il rendering. |
| x | Single | La coordinata X (in pixel) dell'angolo superiore sinistro della pagina renderizzata. |
| y | Single | La coordinata Y (in pixel) dell'angolo superiore sinistro della pagina renderizzata. |

### Vedi anche

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, string) {#toimage_4}

Esegui il rendering di una pagina specifica in un file.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | indica quale pagina deve essere convertita |
| fileName | String | nome file dell'immagine di output |

### Esempi

Il codice seguente genera la prima pagina del primo foglio in immagine png.

```csharp
//carica il file sorgente con le immagini.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//Imposta il tipo di immagine di output.
imgOpt.ImageType = ImageType.Png;

//Renderizza il primo foglio.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//Esporta la prima pagina del foglio in immagine.
sr.ToImage(0, "output.png");
```

### Vedi anche

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Stream) {#toimage_3}

Esegui il rendering di una pagina specifica in uno stream.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | indica quale pagina deve essere convertita |
| stream | Stream | lo stream dell'immagine di output |

### Vedi anche

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int) {#toimage}

Esegui il rendering di una pagina specifica in un oggetto Bitmap.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | indica quale pagina deve essere convertita |

### Valore di ritorno

l'oggetto bitmap della pagina

### Vedi anche

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


