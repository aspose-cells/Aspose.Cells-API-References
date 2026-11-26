---
title: "PageSetup.SetHeader"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Establece un script que formatea el encabezado de un archivo Excel"
type: docs
url: /es/net/aspose.cells/pagesetup/setheader/
---
## PageSetup.SetHeader method

Establece un script que da formato al encabezado de un archivo de Excel.

```csharp
public void SetHeader(int section, string headerScript)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | Int32 | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| headerScript | String | Script de formato de encabezado. |

### Observaciones

Comandos del script:

| **Command** | **Description** |
| --- | --- |
| &amp;P | Número de página actual |
| &amp;N | Recuento de páginas |
| &amp;D | Fecha actual |
| &amp;T | Hora actual |
| &amp;A | Nombre de la hoja |
| &amp;F | Nombre de archivo sin ruta |
| &amp;"&lt;FontName&gt;" | Nombre de fuente, por ejemplo: &amp;"Arial" |
| &amp;"&lt;FontName&gt;, &lt;FontStyle&gt;" | Nombre de fuente y estilo de fuente, por ejemplo: &amp;"Arial,Bold" |
| &amp;&lt;FontSize&gt; | Tamaño de fuente. Si este comando va seguido de un número simple que se imprimirá en el encabezado, se separará de la altura de la fuente con un carácter de espacio. |
| &amp;K&lt;RRGGBB&gt; | Color de fuente, por ejemplo(ROJO): &amp;KFF0000 |
| &amp;G | Script de imagen |

Por ejemplo: "&amp;Arial,Bold&amp;8Header Note"

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Establezca diferentes secciones de encabezado con varios comandos
            pageSetup.SetHeader(0, "&F"); // Left section - File name
            pageSetup.SetHeader(1, "Page &P of &N"); // Center section - Page numbering
            pageSetup.SetHeader(2, "&D"); // Right section - Date

            workbook.Save("PageSetup_SetHeader_Example.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


