---
title: "Clase Style"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridDesktop.Style. Representa el estilo de visualización de documentos de Excel, como color de fuente, alineación, borde, etc."
type: docs
url: /es/net/aspose.cells.griddesktop/style/
---
## Style class

Representa el estilo de visualización de un documento de Excel, como fuente, color, alineación, borde, etc.

```csharp
public class Style
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Style](style/)(GridDesktop) | Crea un nuevo Style para el control |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundColor](../../aspose.cells.griddesktop/style/backgroundcolor/) { get; set; } | Obtiene o establece el color de fondo de la celda, si el patrón de estilo no está configurado como sólido, entonces tendrá efecto. |
| [CellLocked](../../aspose.cells.griddesktop/style/celllocked/) { get; set; } | Obtiene o establece un valor que indica si una celda puede modificarse o no. |
| [Color](../../aspose.cells.griddesktop/style/color/) { get; set; } | Obtiene o establece el color de sombreado de la celda. Cuando el patrón es ninguno, devuelve Color.Empty; cuando el patrón es BackgroundType.Solid, devuelve ForegroundColor; en otros casos devuelve BackgroundColor. |
| [Custom](../../aspose.cells.griddesktop/style/custom/) { get; set; } | Representa la cadena de formato numérico personalizado de este objeto de estilo. Si el formato numérico personalizado no está establecido (Por ejemplo, el formato numérico es incorporado), se devolverá "". |
| [Font](../../aspose.cells.griddesktop/style/font/) { get; set; } | Obtiene un objeto [`GridFont`](../../aspose.cells.griddesktop.data/gridfont/). |
| [ForegroundColor](../../aspose.cells.griddesktop/style/foregroundcolor/) { get; set; } | Obtiene o establece el color de primer plano de un estilo. |
| [HAlignment](../../aspose.cells.griddesktop/style/halignment/) { get; set; } | Obtiene o establece el atributo de alineación horizontal. |
| [Indent](../../aspose.cells.griddesktop/style/indent/) { get; set; } | Representa el nivel m_IndentLevel para la celda o rango. Solo puede ser un entero de 0 a 15. |
| [NumberType](../../aspose.cells.griddesktop/style/numbertype/) { get; set; } | Obtiene o establece el formato de visualización de números y fechas. Los patrones de formato son diferentes según la región. |
| [Pattern](../../aspose.cells.griddesktop/style/pattern/) { get; set; } | Obtiene o establece el tipo de patrón de fondo de la celda. |
| [Rotation](../../aspose.cells.griddesktop/style/rotation/) { get; set; } | Representa el ángulo de rotación del texto. |
| [Shrink](../../aspose.cells.griddesktop/style/shrink/) { get; set; } | Representa si el texto se reduce automáticamente para ajustarse al ancho de columna disponible. |
| [TextDirection](../../aspose.cells.griddesktop/style/textdirection/) { get; set; } | Obtiene o establece el atributo de dirección del texto. |
| [TextWrapped](../../aspose.cells.griddesktop/style/textwrapped/) { get; set; } | Obtiene o establece un valor que indica si el texto dentro de una celda está ajustado. |
| [VAlignment](../../aspose.cells.griddesktop/style/valignment/) { get; set; } | Obtiene o establece el atributo de alineación vertical. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Clone](../../aspose.cells.griddesktop/style/clone/)() | Crea y devuelve una copia de este objeto. **NOTE:** Si clona un estilo con nombre, el nombre no se clona porque el nombre del estilo debe ser único. Por lo tanto, el estilo clonado no será \"igual a\" el estilo original. |
| [SetBorderColor](../../aspose.cells.griddesktop/style/setbordercolor/)(BorderType, Color) | Establece el color del borde especificado. |
| [SetBorderLine](../../aspose.cells.griddesktop/style/setborderline/)(BorderType, BorderLineType) | Establece el tipo de línea del borde especificado. |

### Ver también

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


