---
title: "Enum FontUnderlineType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.FontUnderlineType. Enumera los tipos de subrayado de fuente"
type: docs
url: /es/net/aspose.cells/fontunderlinetype/
---
## FontUnderlineType enumeration

Enumera los tipos de subrayado de fuente.

```csharp
public enum FontUnderlineType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Representa sin subrayado. |
| Single | `1` | Representa subrayado simple. |
| Double | `2` | Representa subrayado doble. |
| Accounting | `3` | Representa subrayado contable simple. |
| DoubleAccounting | `4` | Representa subrayado contable doble. |
| Dash | `5` | Representa subrayado punteado |
| DashDotDotHeavy | `6` | Representa subrayado grueso guión-punto-punto |
| DashDotHeavy | `7` | Representa subrayado grueso guión-punto |
| DashedHeavy | `8` | Representa subrayado grueso punteado |
| DashLong | `9` | Representa subrayado largo punteado |
| DashLongHeavy | `10` | Representa subrayado grueso largo punteado |
| DotDash | `11` | Representa subrayado guión-punto |
| DotDotDash | `12` | Representa subrayado guión-punto-punto |
| Dotted | `13` | Representa subrayado punteado |
| DottedHeavy | `14` | Representa subrayado grueso punteado |
| Heavy | `15` | Representa subrayado grueso |
| Wave | `16` | Representa subrayado ondulado |
| WavyDouble | `17` | Representa subrayado de doble onda |
| WavyHeavy | `18` | Representa subrayado de onda gruesa |
| Words | `19` | Representa subrayado de caracteres que no son espacios. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontUnderlineTypeDemo
    {
        public static void FontUnderlineTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtenga la referencia de la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accediendo a la celda "A1" de la hoja de cálculo
            Cell cell = worksheet.Cells["A1"];
            
            // Añadiendo un valor a la celda "A1"
            cell.PutValue("Hello Aspose!");

            // Obtener el estilo de la celda
            Style style = cell.GetStyle();
            
            // Establecer el tipo de subrayado de fuente a subrayado simple
            style.Font.Underline = FontUnderlineType.Single;
            
            // Aplique el estilo a la celda
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("FontUnderlineTypeExample.xlsx");
            workbook.Save("FontUnderlineTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


