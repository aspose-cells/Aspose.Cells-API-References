---
title: "AutoFitterOptions.DefaultEditLanguage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoFitterOptions. Obtiene o establece el idioma de edición predeterminado"
type: docs
url: /es/net/aspose.cells/autofitteroptions/defaulteditlanguage/
---
## AutoFitterOptions.DefaultEditLanguage property

Obtiene o establece el idioma de edición predeterminado.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Observaciones

Puede mostrar/renderizar diferentes diseños para párrafos de texto cuando se establece un idioma de edición diferente. El predeterminado es Auto.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer texto CJK de muestra en una celda
            worksheet.Cells["A1"].PutValue("日本語のテキスト");

            AutoFitterOptions options = new AutoFitterOptions();
            options.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // Ajustar automáticamente la fila con configuraciones de idioma CJK
            worksheet.AutoFitRows(options);

            Console.WriteLine("Auto-fit completed with DefaultEditLanguage: " + options.DefaultEditLanguage);
            workbook.Save("DefaultEditLanguageDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


