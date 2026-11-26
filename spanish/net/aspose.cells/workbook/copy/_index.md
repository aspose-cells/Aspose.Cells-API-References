---
title: "Workbook.Copy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Copia otro objeto Workbook"
type: docs
url: /es/net/aspose.cells/workbook/copy/
---
## Copy(Workbook, CopyOptions) {#copy_1}

Copia otro objeto Workbook.

```csharp
public void Copy(Workbook source, CopyOptions copyOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | Libro de trabajo | Objeto Workbook de origen. |
| copyOptions | CopyOptions | Las opciones para copiar otro libro de trabajo. |

### Observaciones

Es muy sencillo clonar un archivo Excel.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookCopyOptionsDemo
    {
        public static void Run()
        {
            // Libro de trabajo de origen con macros
            Workbook sourceWorkbook = new Workbook("source_with_macros.xlsm");
            
            // Libro de trabajo de destino (vacío o existente)
            Workbook destWorkbook = new Workbook();
            
            // Configurar opciones de copia para mantener macros
            CopyOptions options = new CopyOptions();
            options.KeepMacros = true;
            
            // Copiar contenido del libro de trabajo de origen al de destino
            sourceWorkbook.Copy(destWorkbook, options);
            
            // Guardar el resultado
            destWorkbook.Save("output_with_macros.xlsm");
        }
    }
}
```

### Ver también

* class [CopyOptions](../../copyoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Workbook) {#copy}

Copia datos de un objeto Workbook fuente.

```csharp
public void Copy(Workbook source)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | Libro de trabajo | Objeto Workbook de origen. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCopyWithWorkbookDemo
    {
        public static void Run()
        {
            // Rutas de archivo de origen y salida
            string sourceFile = "source.xlsx";
            string outputFile = "output.xlsx";

            // Cargar el libro de trabajo de origen
            Workbook sourceWorkbook = new Workbook(sourceFile);

            // Crear un nuevo libro de trabajo y copiar el contenido del origen
            Workbook destinationWorkbook = new Workbook();
            destinationWorkbook.Copy(sourceWorkbook);

            // Guardar el libro de trabajo copiado
            destinationWorkbook.Save(outputFile);
            
            Console.WriteLine("Workbook copied successfully.");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


