---
title: TxtValueQuoteType
second_title: Referencia de API de Aspose.Cells para .NET
description: Especifica el tipo de uso de comillas para valores en archivos de formato de texto.
type: docs
weight: 6140
url: /es/net/aspose.cells/txtvaluequotetype/
---
## TxtValueQuoteType enumeration

Especifica el tipo de uso de comillas para valores en archivos de formato de texto.

```csharp
public enum TxtValueQuoteType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Normal | `0` | Se citarán todos los valores que contengan caracteres especiales como comillas, carácter separador. Igual que el comportamiento de MS Excel para exportar archivos de texto. |
| Always | `1` | Todos los valores se cotizarán siempre. |
| Minimum | `2` | Indique valores solo cuando sea necesario. Por ejemplo, si un valor contiene comillas pero las comillas no están al principio de este valor, este valor no se citará. |
| Never | `3` | No se citarán todos los valores. Es posible que el archivo de texto exportado con este tipo no se lea correctamente porque faltan las comillas necesarias. |

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
