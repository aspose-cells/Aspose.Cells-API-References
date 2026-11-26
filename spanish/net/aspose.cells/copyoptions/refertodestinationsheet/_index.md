---
title: "CopyOptions.ReferToDestinationSheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CopyOptions. Al copiar el rango en el mismo archivo y el gráfico hace referencia a la hoja de origen, False significa que la fuente de datos del gráfico copiado no se cambiará. True significa que la fuente de datos del gráfico copiado hace referencia a la hoja de destino."
type: docs
url: /es/net/aspose.cells/copyoptions/refertodestinationsheet/
---
## CopyOptions.ReferToDestinationSheet property

Al copiar el rango en el mismo archivo y el gráfico hace referencia a la hoja de origen, False significa que la fuente de datos del gráfico copiado no se cambiará. True significa que la fuente de datos del gráfico copiado hará referencia a la hoja de destino.

```csharp
public bool ReferToDestinationSheet { get; set; }
```

### Observaciones

El valor predeterminado es false, funciona como MS Excel. Por ejemplo: si se copia un gráfico con la fuente de datos "sheet1!A1:B10" de la hoja de cálculo "sheet1" a otra hoja "sheet2", la fuente de datos se cambiará a "sheet2!A1:B10".

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToDestinationSheetDemo
    {
        public static void Run()
        {
            // Cree el libro de origen con datos de ejemplo
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B1"].PutValue(100);
            sourceSheet.Cells["A2"].PutValue("=SUM(B1)");

            // Cree un libro de trabajo de destino
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets.Add("DestinationSheet");

            // Establezca las opciones de copia con ReferToDestinationSheet
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ReferToDestinationSheet = true;

            // Copie la hoja de cálculo con las opciones
            destSheet.Copy(sourceSheet, copyOptions);

            // Guardar el resultado
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


