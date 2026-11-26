---
title: "RevisionHeader.SavedTime"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionHeader. Obtiene y establece la fecha y hora cuando se guardó este conjunto de revisiones"
type: docs
url: /es/net/aspose.cells.revisions/revisionheader/savedtime/
---
## RevisionHeader.SavedTime property

Obtiene y establece la fecha y hora en que se guardó este conjunto de revisiones.

```csharp
public DateTime SavedTime { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionHeaderPropertySavedTimeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crea una instancia de RevisionHeader
            RevisionHeader revisionHeader = new RevisionHeader();
            
            try
            {
                // Establece la propiedad SavedTime
                revisionHeader.SavedTime = DateTime.Now;
                
                // Obtén y muestra el valor de SavedTime
                Console.WriteLine("SavedTime value: " + revisionHeader.SavedTime);
                
                // Modifica la propiedad SavedTime
                revisionHeader.SavedTime = DateTime.Now.AddHours(-1);
                Console.WriteLine("Modified SavedTime value: " + revisionHeader.SavedTime);
                
                // Guarda el libro de trabajo para demostrar que la propiedad se está usando
                workbook.Save("SavedTimeDemo.xlsx");
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


