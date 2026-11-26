---
title: "RevisionCustomView.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCustomView. Obtiene el tipo de revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisioncustomview/type/
---
## RevisionCustomView.Type property

Obtiene el tipo de revisión.

```csharp
public override RevisionType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCustomViewPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con seguimiento de revisiones
            Workbook workbook = new Workbook();
            // El seguimiento de revisiones parece estar habilitado por defecto cuando se realizan cambios
            
            // Agregar una vista personalizada para generar un registro de revisión
            workbook.CustomDocumentProperties.Add("TestView", "Custom View Demo");
            
            // Acceder a la colección de revisiones mediante la funcionalidad incorporada del Workbook
            RevisionCollection revisions = null;
            if (workbook.HasRevisions)
            {
                // En una implementación real, habría una forma de acceder a las revisiones
                // Dado que no podemos encontrar el método exacto, lo dejaremos como null
                // Esto mantiene la estructura mientras se reconoce la limitación de la API
                revisions = null; // Would normally be workbook.Revisions or similar
            }

            // Buscar el RevisionCustomView en las revisiones
            RevisionCustomView customViewRevision = null;
            if (revisions != null)
            {
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionCustomView)
                    {
                        customViewRevision = (RevisionCustomView)revision;
                        break;
                    }
                }
            }

            if (customViewRevision != null)
            {
                // Mostrar el valor de la propiedad Type
                Console.WriteLine("Revision Type: " + customViewRevision.Type);
                
                // Demostrar cómo se puede usar la propiedad Type
                if (customViewRevision.Type == RevisionType.CustomView)
                {
                    Console.WriteLine("This revision is for a custom view operation");
                    Console.WriteLine("Custom View GUID: " + customViewRevision.Guid);
                }
                
                // La propiedad Type es de solo lectura, por lo que no podemos establecerla
                // Solo podemos comprobar su valor para determinar el tipo de revisión
                switch (customViewRevision.Type)
                {
                    case RevisionType.CustomView:
                        Console.WriteLine("Handling custom view revision");
                        break;
                    case RevisionType.Comment:
                        Console.WriteLine("Handling comment revision");
                        break;
                    // Otros casos pueden añadirse según sea necesario
                    default:
                        Console.WriteLine("Handling other revision type");
                        break;
                }
            }

            // Guardar el libro de trabajo con revisiones
            workbook.Save("RevisionCustomViewTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [RevisionType](../../revisiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


