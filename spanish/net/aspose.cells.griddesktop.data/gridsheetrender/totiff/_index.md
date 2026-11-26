---
title: "GridSheetRender.ToTiff"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridSheetRender. Renderizar toda la hoja de cálculo como Tiff Image a stream"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridsheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Renderizar toda la hoja de cálculo como imagen Tiff a un flujo.

```csharp
public void ToTiff(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | el flujo de la imagen de salida |

### Ver también

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## ToTiff(string) {#totiff_1}

Renderizar toda la hoja de cálculo como imagen Tiff a un archivo.

```csharp
public void ToTiff(string filename)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre de archivo | String | el nombre de archivo de la imagen de salida |

### Ejemplos

El siguiente código genera todas las páginas de la primera hoja en una imagen Tiff.

```csharp
//cargar el archivo fuente con imágenes.
Workbook wb = new Workbook("Book1.xlsx");

ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();

//establecer el tipo de imagen de salida.
imgOpt.SaveFormat = SaveFormat.Tiff;

//renderizar la primera hoja.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);

//generar todas las páginas de la hoja en una imagen Tiff.
sr.ToTiff("output.tiff");
```

### Ver también

* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


