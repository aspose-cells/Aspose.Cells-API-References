---
title: "PdfSaveOptions.SetImageResample"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PdfSaveOptions. Establece los PPI deseados por pulgada de las imágenes re-muestreadas y la calidad JPEG. Todas las imágenes se convertirán a JPEG con la configuración de calidad especificada y las imágenes que superen los PPI especificados por pulgada serán re-muestreadas"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/setimageresample/
---
## PdfSaveOptions.SetImageResample method

Establece el PPI(píxeles por pulgada) deseado para el remuestreo de imágenes y la calidad JPEG. Todas las imágenes se convertirán a JPEG con la configuración de calidad especificada, y las imágenes que superen el PPI especificado (píxeles por pulgada) serán remuestreadas.

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| desiredPPI | Int32 | Píxeles por pulgada deseados. 220 alta calidad. 150 calidad de pantalla. 96 calidad de correo electrónico. |
| jpegQuality | Int32 | 0 - 100% calidad JPEG. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsMethodSetImageResampleWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook("Book1.xlsx");
            
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.SetImageResample(96, 80);
            
            wb.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


