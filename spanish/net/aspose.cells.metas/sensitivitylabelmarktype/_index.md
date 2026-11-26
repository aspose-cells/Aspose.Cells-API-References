---
title: "Enumeración SensitivityLabelMarkType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Metas.SensitivityLabelMarkType enum. Representa los tipos de marcado de contenido que deben aplicarse a un archivo"
type: docs
url: /es/net/aspose.cells.metas/sensitivitylabelmarktype/
---
## SensitivityLabelMarkType enumeration

Representa los tipos de marcado de contenido que deben aplicarse a un archivo.

```csharp
[Flags]
public enum SensitivityLabelMarkType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Ninguno |
| Header | `1` | Encabezado |
| Footer | `2` | Pie de página |
| Watermark | `4` | Marca de agua |
| Encryption | `8` | Cifrado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelMarkTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demostrar los valores del enum SensitivityLabelMarkType
            SensitivityLabelMarkType markType = SensitivityLabelMarkType.Watermark;

            // Aplicar diferentes marcas de etiqueta de sensibilidad según el tipo
            switch (markType)
            {
                case SensitivityLabelMarkType.None:
                    Console.WriteLine("No sensitivity label applied");
                    break;
                case SensitivityLabelMarkType.Header:
                    worksheet.PageSetup.SetHeader(0, "CONFIDENTIAL");
                    break;
                case SensitivityLabelMarkType.Footer:
                    worksheet.PageSetup.SetFooter(0, "INTERNAL USE ONLY");
                    break;
                case SensitivityLabelMarkType.Watermark:
                    worksheet.PageSetup.SetHeader(0, "&KFF0000&DRAFT");
                    break;
                case SensitivityLabelMarkType.Encryption:
                    workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
                    break;
            }

            // Guardar el libro con la etiqueta de sensibilidad aplicada
            workbook.Save("SensitivityLabelMarkTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


