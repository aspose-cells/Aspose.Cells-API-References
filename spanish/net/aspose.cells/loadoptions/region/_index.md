---
title: "LoadOptions.Region"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Obtiene o establece la configuración regional utilizada para el Workbook que se cargará"
type: docs
url: /es/net/aspose.cells/loadoptions/region/
---
## LoadOptions.Region property

Obtiene o establece la configuración regional utilizada para el Workbook que se cargará.

```csharp
public CountryCode Region { get; set; }
```

### Observaciones

La configuración regional puede usarse para inicializar algunas funciones del libro de trabajo, como fuentes, temas, etc. Para formatos de archivo basados en texto, como CSV, HTML, ..., la configuración regional también se utilizará para detectar formatos numéricos y analizar valores de texto a valores numéricos o de fecha y hora para las celdas. Esta configuración se mantendrá para el libro de trabajo instanciado más adelante, es decir, [`Region`](../../workbooksettings/region/) del libro de trabajo utilizará la misma región que esta propiedad.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyRegionDemo
    {
        public static void Run()
        {
            // Crear opciones de carga para archivo HTML
            LoadOptions loadOpts = new LoadOptions(LoadFormat.Html);
            
            // Establecer la región a USA
            loadOpts.Region = CountryCode.USA;
            
            // Cargar el archivo HTML con la configuración regional especificada
            Workbook wb = new Workbook("example.html", loadOpts);
            
            // Acceder a la primera hoja de cálculo
            Worksheet ws = wb.Worksheets[0];
            
            // Demostrar el formato específico de la región comprobando el estilo de una celda
            Style style = ws.Cells["A1"].GetStyle();
            Console.WriteLine("Font used in cell A1: " + style.Font.Name);
            Console.WriteLine("Region used for loading: " + loadOpts.Region);
        }
    }
}
```

### Ver también

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


