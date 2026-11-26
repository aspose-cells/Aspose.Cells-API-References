---
title: "ExternalLinkCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ExternalLinkCollection. Agrega un enlace externo"
type: docs
url: /es/net/aspose.cells/externallinkcollection/add/
---
## Add(string, string[]) {#add_1}

Agrega un enlace externo.

```csharp
public int Add(string fileName, string[] sheetNames)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | String | El nombre de archivo externo. |
| sheetNames | String[] | Todos los nombres de hoja del archivo externo. |

### Valor de retorno

La posición del nombre externo en esta lista.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithStringStringArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtener la colección de enlaces externos
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Prepare los parámetros para el método Add
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Llame al método Add con los parámetros (String, String[])
                int index = externalLinks.Add(fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");

                // Mostrar información del enlace externo añadido
                ExternalLink link = externalLinks[index];
                Console.WriteLine($"External link file: {link.DataSource}");
                Console.WriteLine("Referenced sheets:");
                foreach (string sheet in sheetNames)
                {
                    Console.WriteLine($"- {sheet}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(DirectoryType, string, string[]) {#add}

Agregar un enlace externo .

```csharp
public int Add(DirectoryType directoryType, string fileName, string[] sheetNames)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directoryType | DirectoryType | El tipo de directorio del nombre de archivo. |
| fileName | String | el nombre de archivo. |
| sheetNames | String[] | Todos los nombres de hoja del archivo externo. |

### Valor de retorno

La posición del nombre externo en esta lista.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionMethodAddWithDirectoryTypeStringStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtener la colección de enlaces externos
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Prepare los parámetros para el método Add
            DirectoryType directoryType = DirectoryType.Volume; // Changed from Directory to Volume
            string fileName = "ExternalWorkbook.xlsx";
            string[] sheetNames = new string[] { "Sheet1", "Sheet2" };

            try
            {
                // Llame al método Add con los parámetros (DirectoryType, String, String[])
                int index = externalLinks.Add(directoryType, fileName, sheetNames);
                
                Console.WriteLine($"External link added at index: {index}");
                Console.WriteLine($"Total external links: {externalLinks.Count}");
                
                // Mostrar información sobre el enlace externo añadido
                ExternalLink link = externalLinks[index];
                Console.WriteLine($"External link references: {link.DataSource}");
                foreach (string sheet in sheetNames) // Changed from link.SheetNames to sheetNames
                {
                    Console.WriteLine($" - References sheet: {sheet}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ExternalLinkCollectionAddDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [DirectoryType](../../directorytype/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


