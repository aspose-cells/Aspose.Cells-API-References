---
title: "WorkbookMetadata.Save"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorkbookMetadata. Guarda los metadatos modificados en el archivo"
type: docs
url: /es/net/aspose.cells.metadata/workbookmetadata/save/
---
## Save(string) {#save_1}

Guarda los metadatos modificados en el archivo.

```csharp
public void Save(string fileName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String | El nombre del archivo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Metadata;

namespace AsposeCellsExamples
{
    public class WorkbookMetadataMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // Crear nuevos metadatos del libro de trabajo
            WorkbookMetadata doc = new WorkbookMetadata("example.xlsb", new MetadataOptions(Aspose.Cells.Metadata.MetadataType.DocumentProperties));
            
            // Agregar propiedades personalizadas
            doc.CustomDocumentProperties.Add("text1", "text2");
            doc.CustomDocumentProperties.Add("num1", 1);
            
            // Guardar con ruta de cadena
            doc.Save("output.xlsb");
            
            // Verifique el archivo guardado
            Workbook workbook = new Workbook("output.xlsb");
            Console.WriteLine("File saved successfully with custom properties.");
            Console.WriteLine("Property 'text1' value: " + doc.CustomDocumentProperties["text1"].Value.ToString());
        }
    }
}
```

### Ver también

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream) {#save}

Guarda los metadatos modificados en el flujo.

```csharp
public void Save(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | El flujo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using System.IO;
    using Aspose.Cells;
    using Aspose.Cells.Metadata;

    public class WorkbookMetadataMethodSaveWithStreamDemo
    {
        public static void Run()
        {
            try
            {
                // Ruta a un libro de trabajo existente (asegúrese de que el archivo exista en la carpeta de ejecución)
                string sourcePath = "Sample.xlsx";

                // Crear MetadataOptions para propiedades de documento
                MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);

                // Instanciar WorkbookMetadata con el archivo fuente y opciones
                WorkbookMetadata metadata = new WorkbookMetadata(sourcePath, options);

                // Acceder a la colección de propiedades de documento incorporada (solo lectura)
                var builtInProperties = metadata.BuiltInDocumentProperties;
                Console.WriteLine("Built‑in document properties collection retrieved.");

                // Guardar los metadatos en un archivo nuevo usando un flujo
                using (FileStream outputStream = new FileStream("MetadataOutput.xlsx",
                                                              FileMode.Create,
                                                              FileAccess.Write))
                {
                    metadata.Save(outputStream);
                }

                Console.WriteLine("Metadata saved successfully to stream.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during metadata Save: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


