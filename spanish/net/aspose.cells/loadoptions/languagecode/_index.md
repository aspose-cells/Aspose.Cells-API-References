---
title: "LoadOptions.LanguageCode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Obtiene o establece el idioma de la interfaz de usuario de la versión del Workbook basado en CountryCode que guardó el archivo"
type: docs
url: /es/net/aspose.cells/loadoptions/languagecode/
---
## LoadOptions.LanguageCode property

Obtiene o establece el idioma de la interfaz de usuario de la versión del Workbook basado en CountryCode que ha guardado el archivo.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Crea una instancia de LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Establecer la propiedad LanguageCode
            loadOptions.LanguageCode = CountryCode.USA;

            // Cargue un libro de trabajo con los LoadOptions especificados
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Acceder a la hoja de cálculo y modificar el contenido
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Language Code Demo");

            // Guardar el libro de trabajo modificado
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


