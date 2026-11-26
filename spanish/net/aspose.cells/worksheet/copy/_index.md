---
title: "Worksheet.Copy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Copia contenidos y formatos de otra hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/copy/
---
## Copy(Worksheet) {#copy}

Copia contenidos y formatos de otra hoja de cálculo.

```csharp
public void Copy(Worksheet sourceSheet)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceSheet | Hoja de cálculo | Hoja de cálculo origen. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetDemo
    {
        public static void Run()
        {
            // Cree un libro de trabajo de origen con datos de muestra
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Worksheet");
            
            // Cree un libro de trabajo de destino
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Copiar la hoja de cálculo origen a la hoja de cálculo destino
            destSheet.Copy(sourceSheet);
            
            // Guardar el resultado
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Worksheet, CopyOptions) {#copy_1}

Copia contenidos y formatos de otra hoja de cálculo.

```csharp
public void Copy(Worksheet sourceSheet, CopyOptions copyOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceSheet | Hoja de cálculo | Hoja de cálculo origen. |
| copyOptions | CopyOptions |  |

### Observaciones

Puede copiar datos de otra hoja de cálculo en el mismo archivo o en otro archivo. Sin embargo, este método no admite copiar objetos de dibujo, como comentarios, imágenes y gráficos.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCopyWithWorksheetCopyOptionsDemo
    {
        public static void Run()
        {
            // Cree el libro de origen con datos de ejemplo
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Name = "SourceSheet";
            srcSheet.Cells["A1"].PutValue("Source Data");

            // Cree un libro de trabajo de destino
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            destSheet.Name = "DestinationSheet";

            // Configurar opciones de copia
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;

            // Copiar hoja de cálculo con opciones
            srcSheet.Copy(destSheet, options);

            // Verificar la operación de copia
            Console.WriteLine("Copied cell value: " + destSheet.Cells["A1"].StringValue);
            
            // Guardar el resultado
            destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [CopyOptions](../../copyoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


