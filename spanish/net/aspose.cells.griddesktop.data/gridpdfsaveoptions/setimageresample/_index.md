---
title: "GridPdfSaveOptions.SetImageResample"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridPdfSaveOptions. Establece los PPI deseados (píxeles por pulgada) de las imágenes re-muestreadas y la calidad JPEG. Todas las imágenes se convertirán a JPEG con la configuración de calidad especificada y las imágenes que superen los PPI especificados se volverán a muestrear"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridpdfsaveoptions/setimageresample/
---
## GridPdfSaveOptions.SetImageResample method

Establece el PPI(píxeles por pulgada) deseado para el remuestreo de imágenes y la calidad JPEG. Todas las imágenes se convertirán a JPEG con la configuración de calidad especificada, y las imágenes que superen el PPI especificado (píxeles por pulgada) serán remuestreadas.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| desiredPPI | Int32 | Píxeles por pulgada deseados. 220 alta calidad. 150 calidad de pantalla. 96 calidad de correo electrónico. |
| jpegQuality | Int32 | 0 - 100% calidad JPEG. |

### Ejemplos

El siguiente código establece los PPI deseados en 96 y la calidad JPEG en 80 para las imágenes en el PDF de salida.

```csharp
//cargar el archivo fuente con imágenes.
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

//establecer los PPI deseados en 96 y la calidad JPEG en 80.
pdfSaveOptions.SetImageResample(96, 80);

wb.Save("output.pdf", pdfSaveOptions);
```

### Ver también

* class [GridPdfSaveOptions](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


