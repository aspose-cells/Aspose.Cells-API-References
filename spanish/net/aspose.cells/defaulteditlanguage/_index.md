---
title: "Enum DefaultEditLanguage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.DefaultEditLanguage enum. Representa el idioma de edición predeterminado"
type: docs
url: /es/net/aspose.cells/defaulteditlanguage/
---
## DefaultEditLanguage enumeration

Representa el idioma de edición predeterminado.

```csharp
public enum DefaultEditLanguage
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Auto | `0` | Representa la detección automática del idioma de edición según el propio texto. |
| English | `1` | Representa el idioma inglés. |
| CJK | `2` | Representa los idiomas chino, japonés y coreano. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultEditLanguageDemo
    {
        public static void DefaultEditLanguageExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea AutoFitterOptions y establece DefaultEditLanguage
            AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
            autoFitterOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // Aplica ajuste automático de filas con las opciones especificadas
            worksheet.AutoFitRows(autoFitterOptions);

            // Guarda el libro de trabajo
            workbook.Save("DefaultEditLanguageExample.xlsx");
            workbook.Save("DefaultEditLanguageExample.pdf");

            // Muestra en la consola el DefaultEditLanguage configurado
            Console.WriteLine("Default Edit Language set to: " + autoFitterOptions.DefaultEditLanguage);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


