---
title: "XlsSaveOptions.WpsCompatibility"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de XlsSaveOptions. Indica si se debe hacer el xls más compatible con WPS"
type: docs
url: /es/net/aspose.cells/xlssaveoptions/wpscompatibility/
---
## XlsSaveOptions.WpsCompatibility property

Indica si se debe hacer el xls más compatible con WPS.

```csharp
[Obsolete("Use WorkbookSetting.WpsCompatibility property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool WpsCompatibility { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad WorkbookSetting.WpsCompatibility. Este método será eliminado 12 meses después desde diciembre de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyWpsCompatibilityDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Test WPS Compatibility");
            worksheet.Cells["B1"].PutValue(123.45);
            
            // Establecer opciones de guardado con compatibilidad WPS
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.WpsCompatibility = true;
            
            // Guarda el libro de trabajo
            workbook.Save("output_with_wps_compatibility.xls", saveOptions);
            
            Console.WriteLine("File saved with WPS compatibility enabled.");
        }
    }
}
```

### Ver también

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


