---
title: "WorkbookMetadata.Options"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookMetadata. Obtiene las opciones de los metadatos"
type: docs
url: /es/net/aspose.cells.metadata/workbookmetadata/options/
---
## WorkbookMetadata.Options property

Obtiene las opciones de los metadatos.

```csharp
public MetadataOptions Options { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class WorkbookMetadataPropertyOptionsDemo
    {
        public static void Run()
        {
            // Crear opciones de metadatos para propiedades de documento
            MetadataOptions options = new MetadataOptions(MetadataType.DocumentProperties);
            options.Password = "test123";
            options.KeyLength = 128;

            // Crear una nueva instancia de metadatos del libro de trabajo con opciones
            WorkbookMetadata metadata = new WorkbookMetadata("sample.xlsx", options);

            // Mostrar valores actuales de las opciones
            Console.WriteLine("Metadata Type: " + metadata.Options.MetadataType);
            Console.WriteLine("Password: " + metadata.Options.Password);
            Console.WriteLine("Key Length: " + metadata.Options.KeyLength);

            // Acceder a las propiedades de documento incorporadas
            var builtInProps = metadata.BuiltInDocumentProperties;
            builtInProps.Author = "Aspose Developer";
            builtInProps.Title = "Metadata Demo";

            // Agregar propiedades de documento personalizadas
            var customProps = metadata.CustomDocumentProperties;
            customProps.Add("Department", "Development");
            customProps.Add("Project", "Metadata API");

            // Guardar los cambios de los metadatos
            metadata.Save("output.xlsx");

            // Crear nuevas opciones para el cifrado
            MetadataOptions newOptions = new MetadataOptions(MetadataType.Encryption);
            newOptions.Password = "newpassword";
            newOptions.KeyLength = 256;
            
            WorkbookMetadata encryptedMetadata = new WorkbookMetadata("sample.xlsx", newOptions);
            encryptedMetadata.Save("encrypted_output.xlsx");
        }
    }
}
```

### Ver también

* class [MetadataOptions](../../metadataoptions/)
* class [WorkbookMetadata](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


