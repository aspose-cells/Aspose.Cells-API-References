---
title: "RevisionCustomView.ActionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionCustomView. Obtiene el tipo de acción"
type: docs
url: /es/net/aspose.cells.revisions/revisioncustomview/actiontype/
---
## RevisionCustomView.ActionType property

Obtiene el tipo de acción.

```csharp
public RevisionActionType ActionType { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCustomViewPropertyActionTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Cargar un workbook existente que podría contener revisiones de vista personalizada
                Workbook workbook = new Workbook("SampleWithRevisions.xlsx");

                // Iterar a través de todos los registros de revisión en el workbook
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    // Comprobar cada revisión en el registro
                    foreach (Revision revision in log.Revisions)
                    {
                        // Verificar si esto es una revisión de vista personalizada
                        if (revision is RevisionCustomView)
                        {
                            RevisionCustomView customViewRevision = (RevisionCustomView)revision;

                            // Muestre el valor de la propiedad ActionType
                            Console.WriteLine($"Custom View Revision Action Type: {customViewRevision.ActionType}");

                            // Demostrar cómo usar la propiedad ActionType
                            switch (customViewRevision.ActionType)
                            {
                                case RevisionActionType.Add:
                                    Console.WriteLine("This revision represents adding a custom view");
                                    break;
                                case RevisionActionType.Delete:
                                    Console.WriteLine("This revision represents deleting a custom view");
                                    break;
                                default:
                                    Console.WriteLine("This revision represents another type of action");
                                    break;
                            }

                            // Mostrar propiedades adicionales para contexto
                            Console.WriteLine($"Revision Type: {customViewRevision.Type}");
                            Console.WriteLine($"Custom View GUID: {customViewRevision.Guid}");
                        }
                    }
                }
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

* enum [RevisionActionType](../../revisionactiontype/)
* class [RevisionCustomView](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


