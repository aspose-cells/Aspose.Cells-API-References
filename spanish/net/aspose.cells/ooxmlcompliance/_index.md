---
title: "Enum OoxmlCompliance"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.OoxmlCompliance enum. Permite especificar qué especificación OOXML se utilizará al guardar en formato Xlsx."
type: docs
url: /es/net/aspose.cells/ooxmlcompliance/
---
## OoxmlCompliance enumeration

Permite especificar qué especificación OOXML se utilizará al guardar en formato Xlsx.

```csharp
public enum OoxmlCompliance
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Ecma376_2006 | `0` | ECMA-376 1st Edition, 2006. |
| Iso29500_2008_Strict | `1` | Nivel de cumplimiento estricto ISO/IEC 29500:2008. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlComplianceDemo
    {
        public static void OoxmlComplianceExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Establecer el nivel de cumplimiento OOXML a ISO/IEC 29500:2008 Strict
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;

            // Agregar algunos datos a la hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, World!");

            // Guardar el libro de trabajo con el nivel de cumplimiento OOXML especificado
            workbook.Save("OoxmlComplianceExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


