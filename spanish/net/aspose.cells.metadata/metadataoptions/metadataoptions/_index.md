---
title: "MetadataOptions.MetadataOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "MetadataOptions constructor. Crea una opción para cargar los metadatos"
type: docs
url: /es/net/aspose.cells.metadata/metadataoptions/metadataoptions/
---
## MetadataOptions constructor

Crea una opción para cargar los metadatos.

```csharp
public MetadataOptions(MetadataType metadataType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| metadataType | MetadataType | El tipo de metadatos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metadata;
    using System;

    public class MetadataOptionsMethodCtorWithMetadataTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Llame al método #ctor con el parámetro MetadataType
                MetadataOptions options = new MetadataOptions(MetadataType.Encryption);
                
                // Establecer propiedades adicionales
                options.Password = "test123";
                options.KeyLength = 128;
                
                // Mostrar las opciones creadas
                Console.WriteLine($"MetadataType: {options.MetadataType}");
                Console.WriteLine($"Password set: {!string.IsNullOrEmpty(options.Password)}");
                Console.WriteLine($"KeyLength: {options.KeyLength}");

                // Utilice las opciones al cargar metadatos (ejemplo)
                // Esto normalmente se usaría con LoadOptions al abrir un archivo
                // Nota: El código original intentó establecer MetadataOptions directamente en LoadOptions,
                // pero la clase LoadOptions no tiene esta propiedad en la definición proporcionada.
                // Simplemente mantendremos la parte de creación de opciones ya que el uso con LoadOptions
                // no es posible con la definición actual de la API.
                
                Console.WriteLine("MetadataOptions created successfully with MetadataType parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating MetadataOptions: {ex.Message}");
            }
            
            // Guarda el libro de trabajo (aunque las opciones de metadatos no afectarían a este libro de trabajo vacío)
            workbook.Save("MetadataOptionsCtorDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MetadataType](../../metadatatype/)
* class [MetadataOptions](../)
* namespace [Aspose.Cells.Metadata](../../../aspose.cells.metadata/)
* assembly [Aspose.Cells](../../../)


