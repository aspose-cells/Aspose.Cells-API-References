---
title: "Workbook.Combine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método del libro de trabajo. Combina otro objeto Workbook"
type: docs
url: /es/net/aspose.cells/workbook/combine/
---
## Workbook.Combine method

Combina otro objeto Workbook.

```csharp
public void Combine(Workbook secondWorkbook)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| secondWorkbook | Libro de trabajo | Otro objeto Workbook. |

### Observaciones

Combine Excel, ODS, CSV y otros archivos en un solo archivo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCombineWithWorkbookDemo
    {
        public static void Run()
        {
            // Cree el libro de trabajo fuente
            Workbook sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets[0].Cells["A1"].PutValue("Source Data");

            // Cree un libro de trabajo de destino
            Workbook destWorkbook = new Workbook(FileFormatType.Xlsx);
            destWorkbook.Worksheets[0].Cells["B2"].PutValue("Destination Data");

            // Combine los libros de trabajo
            destWorkbook.Combine(sourceWorkbook);

            // Guarde el libro de trabajo combinado
            destWorkbook.Save("CombinedWorkbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


