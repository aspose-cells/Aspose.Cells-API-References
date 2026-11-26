---
title: "Clase CopyOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CopyOptions. Representa las opciones de copia"
type: docs
url: /es/net/aspose.cells/copyoptions/
---
## CopyOptions class

Representa las opciones de copia.

```csharp
public class CopyOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CopyOptions](copyoptions/)() | Constructor de CopyOptions. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ColumnCharacterWidth](../../aspose.cells/copyoptions/columncharacterwidth/) { get; set; } | Indica si se copia el ancho de columna en unidades de caracteres. |
| [CopyInvalidFormulasAsValues](../../aspose.cells/copyoptions/copyinvalidformulasasvalues/) { get; set; } | Si la fórmula no es válida para el destino, solo copiar valores. |
| [CopyNames](../../aspose.cells/copyoptions/copynames/) { get; set; } | Indica si se copian los nombres. |
| [ExtendToAdjacentRange](../../aspose.cells/copyoptions/extendtoadjacentrange/) { get; set; } | Indica si se extienden los rangos al copiar el rango a un rango adyacente. |
| [KeepMacros](../../aspose.cells/copyoptions/keepmacros/) { get; set; } | Indica si se conservan las macros; |
| [ReferToDestinationSheet](../../aspose.cells/copyoptions/refertodestinationsheet/) { get; set; } | Al copiar el rango en el mismo archivo y el gráfico hace referencia a la hoja de origen, False significa que la fuente de datos del gráfico copiado no se cambiará. True significa que la fuente de datos del gráfico copiado hará referencia a la hoja de destino. |
| [ReferToSheetWithSameName](../../aspose.cells/copyoptions/refertosheetwithsamename/) { get; set; } | En MS Excel, al copiar fórmulas que hacen referencia a otras hojas de cálculo mientras se copia una hoja a otra, las fórmulas copiadas deben referirse al libro de origen. Sin embargo, en algunas situaciones el usuario puede necesitar que las fórmulas copiadas hagan referencia a hojas con el mismo nombre en el mismo libro, como cuando esas hojas ya fueron copiadas antes de esta operación de copia, entonces esta propiedad debe mantenerse como true. |
| [UpdateInvalidReferencesToTargetSheet](../../aspose.cells/copyoptions/updateinvalidreferencestotargetsheet/) { get; set; } | Indica si se debe referir a la hoja de cálculo de destino si la hoja referenciada no se copia. |

### Ejemplos

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CopyOptionsDemo
    {
        public static void CopyOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");

            // Crear un nuevo libro de trabajo donde copiar los datos
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Crear un objeto CopyOptions
            CopyOptions copyOptions = new CopyOptions
            {
                KeepMacros = true,
                ExtendToAdjacentRange = true,
                CopyNames = true,
                CopyInvalidFormulasAsValues = true,
                ColumnCharacterWidth = true,
                ReferToSheetWithSameName = true,
                ReferToDestinationSheet = true
            };

            // Copiar los datos de la hoja de cálculo origen a la hoja de cálculo destino
            destSheet.Cells.CopyRows(sheet.Cells, 0, 0, 2, copyOptions);

            // Guardar el libro de trabajo de destino
            destWorkbook.Save("CopyOptionsExample.xlsx");
            destWorkbook.Save("CopyOptionsExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


