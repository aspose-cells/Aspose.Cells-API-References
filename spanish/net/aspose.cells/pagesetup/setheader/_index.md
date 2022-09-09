---
title: SetHeader
second_title: Referencia de API de Aspose.Cells para .NET
description: Establece un script que formatea el encabezado de un archivo de Excel.
type: docs
weight: 620
url: /es/net/aspose.cells/pagesetup/setheader/
---
## PageSetup.SetHeader method

Establece un script que formatea el encabezado de un archivo de Excel.

```csharp
public void SetHeader(int section, string headerScript)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| section | Int32 | 0: Sección izquierda, 1: Sección central, 2: Sección derecha. |
| headerScript | String | Script de formato de encabezado. |

### Observaciones

Comandos de guión:

**Dominio**

**Descripción**

&amp;PAGS

Número de página actual

&amp;NORTE

Recuento de páginas

&amp;D

Fecha actual

&amp;T

Tiempo actual

&amp;A

Nombre de la hoja

&amp;F

Nombre de archivo sin ruta

&amp;"&lt;Nombre de fuente&gt;"

Nombre de fuente, por ejemplo: &amp;"Arial"

&amp;"&lt;Nombre de fuente&gt;, &lt;Estilo de fuente&gt;"

Nombre de fuente y estilo de fuente, por ejemplo: &amp;"Arial,Negrita"

&amp;&lt;Tamaño de fuente&gt;

Tamaño de fuente. Si este comando es seguido por un número simple que se imprimirá en el encabezado, se separará de la altura de la fuente con un carácter de espacio.

&amp;K&lt;RRGGBB&gt;

Color de fuente, por ejemplo (ROJO): &amp;KFF0000

&amp;GRAMO

Guión de imagen

Por ejemplo: "&amp;Arial,Negrita&amp;8Nota de encabezado"

### Ver también

* class [PageSetup](../../pagesetup)
* espacio de nombres [Aspose.Cells](../../pagesetup)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->