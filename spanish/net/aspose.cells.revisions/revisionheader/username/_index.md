---
title: "RevisionHeader.UserName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionHeader. Obtiene y establece el nombre del usuario que realiza la revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisionheader/username/
---
## RevisionHeader.UserName property

Obtiene y establece el nombre del usuario que realiza la revisión.

```csharp
public string UserName { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertyUserNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            try
            {
                // Crea una instancia de RevisionHeader
                RevisionHeader revisionHeader = new RevisionHeader();

                // Establece la propiedad UserName
                revisionHeader.UserName = "JohnDoe";

                // Muestra el valor actual de la propiedad UserName
                Console.WriteLine("UserName value: " + revisionHeader.UserName);

                // Modifica la propiedad UserName
                revisionHeader.UserName = "JaneSmith";
                Console.WriteLine("Modified UserName value: " + revisionHeader.UserName);

                // Guarda el libro de trabajo para demostrar que la propiedad se está usando
                workbook.Save("UserNameDemo.xlsx");
                Console.WriteLine("UserName property has been demonstrated and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [RevisionHeader](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


