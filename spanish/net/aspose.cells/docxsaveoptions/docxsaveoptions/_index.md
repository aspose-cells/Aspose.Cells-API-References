---
title: "DocxSaveOptions.DocxSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor DocxSaveOptions. Representa opciones para guardar un archivo .docx"
type: docs
url: /es/net/aspose.cells/docxsaveoptions/docxsaveoptions/
---
## DocxSaveOptions() {#constructor}

Representa las opciones para guardar un archivo .docx.

```csharp
public DocxSaveOptions()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo y agregue datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Inicialice DocxSaveOptions usando el constructor
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.SaveAsEditableShaps = true;
            
            // Guarde el libro de trabajo como DOCX con opciones
            workbook.Save("output.docx", saveOptions);
            
            Console.WriteLine("Document saved successfully with DocxSaveOptions.");
        }
    }
}
```

### Ver también

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DocxSaveOptions(bool) {#constructor_1}

Representa las opciones para guardar un archivo .docx.

```csharp
public DocxSaveOptions(bool saveAsImage)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| saveAsImage | Booleano | Si True, el libro de trabajo se convertirá en algunas imágenes del archivo .docx. Si False, el libro de trabajo se convertirá en algunas tablas del archivo .docx. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Guardar como DOCX con opciones predeterminadas
            workbook.Save("output_default.docx");
            
            // Guardar como DOCX con DocxSaveOptions(true) - optimizado para MS Word
            workbook.Save("output_optimized.docx", new DocxSaveOptions(true));
        }
    }
}
```

### Ver también

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


