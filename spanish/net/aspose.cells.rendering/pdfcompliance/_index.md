---
title: "Enum PdfCompliance"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Rendering.PdfCompliance. Permite al usuario establecer la compatibilidad de conversiones PDF"
type: docs
url: /es/net/aspose.cells.rendering/pdfcompliance/
---
## PdfCompliance enumeration

Permitiendo al usuario establecer la compatibilidad de la conversión PDF.

```csharp
public enum PdfCompliance
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Formato PDF compatible con PDF 1.4 |
| Pdf14 | `0` | Formato PDF compatible con PDF 1.4 |
| Pdf15 | `3` | Formato PDF compatible con PDF 1.5 |
| Pdf16 | `4` | Formato PDF compatible con PDF 1.6 |
| Pdf17 | `5` | Formato PDF compatible con PDF 1.7 |
| PdfA1b | `1` | Formato PDF compatible con PDF/A-1b (ISO 19005-1) |
| PdfA1a | `2` | Formato PDF compatible con PDF/A-1a (ISO 19005-1) |
| PdfA2b | `6` | Formato PDF compatible con PDF/A-2b (ISO 19005-2) |
| PdfA2u | `7` | Formato PDF compatible con PDF/A-2u (ISO 19005-2) |
| PdfA2a | `8` | Formato PDF compatible con PDF/A-2a (ISO 19005-2) |
| PdfA3b | `9` | Formato PDF compatible con PDF/A-3b (ISO 19005-3) |
| PdfA3u | `10` | Formato PDF compatible con PDF/A-3u (ISO 19005-3) |
| PdfA3a | `11` | Formato PDF compatible con PDF/A-3a (ISO 19005-3) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfComplianceDemo
    {
        public static void PdfComplianceExample()
        {
            // Creando un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Compliance Example");

            // Configurando opciones de guardado PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();

            // Estableciendo el nivel de cumplimiento a PDF/A-1b
            saveOptions.Compliance = PdfCompliance.PdfA1b;

            // Guardando el libro de trabajo en PDF con el nivel de cumplimiento especificado
            workbook.Save("PdfComplianceExample.pdf", saveOptions);

            Console.WriteLine("PDF generated with compliance level PDF/A-1b");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


