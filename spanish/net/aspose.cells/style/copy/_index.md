---
title: "Style.Copy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Style. Copia datos de otro objeto de estilo"
type: docs
url: /es/net/aspose.cells/style/copy/
---
## Style.Copy method

Copia datos de otro objeto de estilo

```csharp
public void Copy(Style style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | Objeto Style de origen |

### Observaciones

Este método no copia el nombre del estilo. Si desea copiar el nombre, por favor llame al siguiente código después de copiar el estilo: destStyle.Name = style.Name.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCopyWithStyleDemo
    {
        public static void Run()
        {
            // Cree el libro de origen con datos de ejemplo
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Sample Text");
            Style srcStyle = srcWorkbook.CreateStyle();
            srcStyle.Font.Name = "Arial";
            srcStyle.Font.Size = 14;
            srcSheet.Cells["A1"].SetStyle(srcStyle);

            // Cree un libro de trabajo de destino
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Copiar el estilo del origen al destino
            Style destStyle = destWorkbook.CreateStyle();
            destStyle.Copy(srcStyle);
            
            // Aplicar el estilo copiado
            destSheet.Cells["B2"].PutValue("Copied Style Text");
            destSheet.Cells["B2"].SetStyle(destStyle);

            // Guardar el resultado
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


