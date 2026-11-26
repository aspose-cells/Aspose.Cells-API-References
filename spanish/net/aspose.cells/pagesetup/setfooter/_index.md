---
title: "PageSetup.SetFooter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Establece un script que formatea el pie de página de un archivo Excel"
type: docs
url: /es/net/aspose.cells/pagesetup/setfooter/
---
## PageSetup.SetFooter method

Establece un script que da formato al pie de página de un archivo de Excel.

```csharp
public void SetFooter(int section, string footerScript)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| section | Int32 | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| footerScript | String | Script de formato de pie de página. |

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

Por ejemplo: "&amp;Arial,Bold&amp;8Footer Note"

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFooterWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.SetFooter(0, "Page &P");
            worksheet.PageSetup.SetFooter(1, "&D");
            worksheet.PageSetup.SetFooter(2, "&A");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


