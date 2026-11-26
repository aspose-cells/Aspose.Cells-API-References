---
title: "Enumeración NumberCategoryType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.NumberCategoryType enum. Representa el tipo de categoría del formato numérico de las celdas"
type: docs
url: /es/net/aspose.cells/numbercategorytype/
---
## NumberCategoryType enumeration

Representa el tipo de categoría del formato numérico de la celda.

```csharp
public enum NumberCategoryType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| General | `0` | General |
| Text | `1` | Texto |
| Number | `2` | Número |
| Date | `3` | Fecha o Fecha y hora |
| Time | `4` | Hora |
| Fraction | `5` | Fracción |
| Scientific | `6` | Científico |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NumberCategoryTypeDemo
    {
        public static void NumberCategoryTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("General");
            worksheet.Cells["A2"].PutValue("Text");
            worksheet.Cells["A3"].PutValue(12345);
            worksheet.Cells["A4"].PutValue(DateTime.Now);
            worksheet.Cells["A5"].PutValue(TimeSpan.FromHours(1.5));
            worksheet.Cells["A6"].PutValue(0.75);
            worksheet.Cells["A7"].PutValue(1.23E+3);

            // Establecer formatos numéricos para las celdas
            worksheet.Cells["A1"].SetStyle(CreateStyle(workbook, NumberCategoryType.General));
            worksheet.Cells["A2"].SetStyle(CreateStyle(workbook, NumberCategoryType.Text));
            worksheet.Cells["A3"].SetStyle(CreateStyle(workbook, NumberCategoryType.Number));
            worksheet.Cells["A4"].SetStyle(CreateStyle(workbook, NumberCategoryType.Date));
            worksheet.Cells["A5"].SetStyle(CreateStyle(workbook, NumberCategoryType.Time));
            worksheet.Cells["A6"].SetStyle(CreateStyle(workbook, NumberCategoryType.Fraction));
            worksheet.Cells["A7"].SetStyle(CreateStyle(workbook, NumberCategoryType.Scientific));

            // Mostrar los tipos de categoría numérica
            Console.WriteLine("Cell A1 Number Category Type: " + worksheet.Cells["A1"].NumberCategoryType);
            Console.WriteLine("Cell A2 Number Category Type: " + worksheet.Cells["A2"].NumberCategoryType);
            Console.WriteLine("Cell A3 Number Category Type: " + worksheet.Cells["A3"].NumberCategoryType);
            Console.WriteLine("Cell A4 Number Category Type: " + worksheet.Cells["A4"].NumberCategoryType);
            Console.WriteLine("Cell A5 Number Category Type: " + worksheet.Cells["A5"].NumberCategoryType);
            Console.WriteLine("Cell A6 Number Category Type: " + worksheet.Cells["A6"].NumberCategoryType);
            Console.WriteLine("Cell A7 Number Category Type: " + worksheet.Cells["A7"].NumberCategoryType);

            // Guarda el libro de trabajo
            workbook.Save("NumberCategoryTypeExample.xlsx");
        }

        private static Style CreateStyle(Workbook workbook, NumberCategoryType numberCategoryType)
        {
            Style style = workbook.CreateStyle();
            switch (numberCategoryType)
            {
                case NumberCategoryType.General:
                    style.Number = 0;
                    break;
                case NumberCategoryType.Text:
                    style.Number = 49;
                    break;
                case NumberCategoryType.Number:
                    style.Number = 1;
                    break;
                case NumberCategoryType.Date:
                    style.Number = 14;
                    break;
                case NumberCategoryType.Time:
                    style.Number = 21;
                    break;
                case NumberCategoryType.Fraction:
                    style.Number = 9;
                    break;
                case NumberCategoryType.Scientific:
                    style.Number = 11;
                    break;
            }
            return style;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


