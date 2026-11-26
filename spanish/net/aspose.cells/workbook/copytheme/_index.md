---
title: "Workbook.CopyTheme"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Copia el tema de otro workbook"
type: docs
url: /es/net/aspose.cells/workbook/copytheme/
---
## Workbook.CopyTheme method

Copia el tema de otro libro de trabajo.

```csharp
public void CopyTheme(Workbook source)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | Libro de trabajo | Libro de trabajo de origen. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyThemeWithWorkbookDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo de origen (el tema se establece automáticamente al abrir un archivo de plantilla)
            Workbook sourceWorkbook = new Workbook(FileFormatType.Xlsx);

            // Cree un libro de trabajo de destino
            Workbook destWorkbook = new Workbook();
            
            // Copiar el tema del libro de trabajo de origen al libro de trabajo de destino
            destWorkbook.CopyTheme(sourceWorkbook);

            // Guardar el libro de trabajo de destino
            destWorkbook.Save("output_with_theme.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


