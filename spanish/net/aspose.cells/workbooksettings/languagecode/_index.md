---
title: "WorkbookSettings.LanguageCode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene o establece el idioma de la interfaz de usuario de la versión del libro de trabajo basado en CountryCode que guardó el archivo"
type: docs
url: /es/net/aspose.cells/workbooksettings/languagecode/
---
## WorkbookSettings.LanguageCode property

Obtiene o establece el idioma de la interfaz de usuario de la versión del Workbook basado en CountryCode que ha guardado el archivo.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Establecer el código de idioma a Alemán (Alemania)
            settings.LanguageCode = CountryCode.Germany;

            // Mostrar el código de idioma actual
            Console.WriteLine("Current Language Code: " + settings.LanguageCode);

            // Cambiar el código de idioma a Francés (Francia)
            settings.LanguageCode = CountryCode.France;
            Console.WriteLine("Updated Language Code: " + settings.LanguageCode);

            // Guarda el libro de trabajo
            workbook.Save("WorkbookSettings_LanguageCodeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


