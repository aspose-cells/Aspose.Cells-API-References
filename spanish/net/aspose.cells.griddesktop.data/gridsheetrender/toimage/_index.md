---
title: "GridSheetRender.ToImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridSheetRender. Renderiza una página determinada a un Graphics"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridsheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Renderizar una página determinada a un Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | indicar qué página se va a convertir |
| g | Graphics | El objeto donde renderizar. |
| x | Single | La coordenada X (en píxeles) de la esquina superior izquierda de la página renderizada. |
| y | Single | La coordenada Y (en píxeles) de la esquina superior izquierda de la página renderizada. |
| ancho | Single | El ancho máximo (en píxeles) que puede ocupar la página renderizada. |
| altura | Single | La altura máxima (en píxeles) que puede ocupar la página renderizada. |

### Ver también

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Renderizar una página determinada a un Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | indicar qué página se va a convertir |
| g | Graphics | El objeto donde renderizar. |
| x | Single | La coordenada X (en píxeles) de la esquina superior izquierda de la página renderizada. |
| y | Single | La coordenada Y (en píxeles) de la esquina superior izquierda de la página renderizada. |

### Ver también

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, string) {#toimage_4}

Renderizar una página específica a un archivo.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | indicar qué página se va a convertir |
| fileName | String | nombre de archivo de la imagen de salida |

### Ejemplos

El siguiente código genera la primera página de la primera hoja en una imagen png.

```csharp
//cargar el archivo fuente con imágenes.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//establecer el tipo de imagen de salida.
imgOpt.ImageType = ImageType.Png;

//renderizar la primera hoja.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//generar la primera página de la hoja en una imagen.
sr.ToImage(0, "output.png");
```

### Ver también

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int, Stream) {#toimage_3}

Renderizar una página específica a un flujo.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | indicar qué página se va a convertir |
| stream | Stream | el flujo de la imagen de salida |

### Ver también

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToImage(int) {#toimage}

Renderizar una página específica a un objeto Bitmap.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | indicar qué página se va a convertir |

### Valor de retorno

el objeto bitmap de la página

### Ver también

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


