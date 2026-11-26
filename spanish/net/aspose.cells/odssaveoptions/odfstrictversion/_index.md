---
title: "OdsSaveOptions.OdfStrictVersion"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsSaveOptions. Obtiene y establece la versión ODF"
type: docs
url: /es/net/aspose.cells/odssaveoptions/odfstrictversion/
---
## OdsSaveOptions.OdfStrictVersion property

Obtiene y establece la versión ODF.

```csharp
public OpenDocumentFormatVersionType OdfStrictVersion { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyOdfStrictVersionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ODF Version Demo");

            // Crear opciones de guardado ODS
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            
            // Establecer la versión ODF a 1.2
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // Guardar con la versión ODF especificada
            workbook.Save("OdfVersion12.ods", saveOptions);

            // Cambiar a la versión ODF 1.3
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf13;
            workbook.Save("OdfVersion13.ods", saveOptions);
        }
    }
}
```

### Ver también

* enum [OpenDocumentFormatVersionType](../../../aspose.cells.ods/opendocumentformatversiontype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


