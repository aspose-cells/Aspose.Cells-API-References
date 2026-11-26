---
title: "DocxSaveOptions.SaveAsEditableShaps"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DocxSaveOptions. Guardar todos los objetos de dibujo como formas editables en el archivo Word. Así puede editarlos en Word"
type: docs
url: /es/net/aspose.cells/docxsaveoptions/saveaseditableshaps/
---
## DocxSaveOptions.SaveAsEditableShaps property

Guardar todos los objetos de dibujo como formas editables en el archivo Word. Así puede editarlos en Word.

```csharp
[Obsolete("Use SaveFormat.SaveAsEditableShapes instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SaveAsEditableShaps { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad [`SaveAsEditableShapes`](../saveaseditableshapes/). Esta propiedad será eliminada 6 meses después desde mayo de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveAsEditableShapsDemo
    {
        public static void Run()
        {
            // Crear un objeto de libro de trabajo y abrir el archivo Excel plantilla
            Workbook workbook = new Workbook("example.xlsx");

            // Inicialice DocxSaveOptions
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            
            // Establecer la propiedad SaveAsEditableShaps a true
            saveOptions.SaveAsEditableShaps = true;

            // Guardar el libro de trabajo como DOCX con las opciones especificadas
            workbook.Save("example.docx", saveOptions);
        }
    }
}
```

### Ver también

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


