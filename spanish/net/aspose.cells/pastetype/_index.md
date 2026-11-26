---
title: "Enum PasteType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.PasteType. Representa el tipo de pegado especial"
type: docs
url: /es/net/aspose.cells/pastetype/
---
## PasteType enumeration

Representa el tipo de pegado especial.

```csharp
public enum PasteType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| All | `0` | Copia todos los datos del rango. |
| Default | `1` | Funciona como el comportamiento "All" de MS Excel. |
| AllExceptBorders | `2` | Copia todos los datos del rango sin el rango. |
| DefaultExceptBorders | `3` | Funciona como el comportamiento "All except borders" de MS Excel. |
| ColumnWidths | `4` | Solo copia los anchos del rango. |
| RowHeights | `5` | Solo copia las alturas del rango. |
| Comments | `6` | Solo copia los comentarios en el rango. |
| Formats | `7` | Solo copia los formatos en el rango. |
| Formulas | `8` | Solo copia fórmulas en el rango. |
| FormulasAndNumberFormats | `9` | Solo copia fórmulas y formatos numéricos en el rango. |
| Validation | `10` | Solo copia validaciones en el rango. |
| Values | `11` | Solo copia valores en el rango. |
| ValuesAndFormats | `12` | Solo copia valores y formatos en el rango. |
| ValuesAndNumberFormats | `13` | Solo copia valores y formatos numéricos en el rango. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteTypeDemo
    {
        public static void PasteTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Defina el rango de origen
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B4");

            // Defina el rango de destino
            Aspose.Cells.Range destinationRange = worksheet.Cells.CreateRange("D1:E4");

            // Cree PasteOptions y establezca PasteType
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                IgnoreLinksToOriginalFile = true
            };

            // Copie el rango de origen al rango de destino con las PasteOptions especificadas
            destinationRange.Copy(sourceRange, pasteOptions);

            // Guarda el libro de trabajo
            workbook.Save("PasteTypeExample.xlsx");

            // Genere la salida de los resultados
            Console.WriteLine("Data copied with PasteType.Values and saved to PasteTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


