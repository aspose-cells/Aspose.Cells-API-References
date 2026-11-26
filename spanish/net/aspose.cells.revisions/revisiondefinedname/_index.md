---
title: "Clase RevisionDefinedName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Revisions.RevisionDefinedName. Representa un registro de revisión de un cambio de nombre definido"
type: docs
url: /es/net/aspose.cells.revisions/revisiondefinedname/
---
## RevisionDefinedName class

Representa un registro de revisión de un cambio de nombre definido.

```csharp
public class RevisionDefinedName : Revision
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Obtiene el número de esta revisión.(Heredado de [`Revision`](../revision/).) |
| [NewFormula](../../aspose.cells.revisions/revisiondefinedname/newformula/) { get; } | Obtiene la fórmula. |
| [OldFormula](../../aspose.cells.revisions/revisiondefinedname/oldformula/) { get; } | Obtiene la fórmula anterior. |
| [Text](../../aspose.cells.revisions/revisiondefinedname/text/) { get; } | Obtiene el texto del nombre definido. |
| override [Type](../../aspose.cells.revisions/revisiondefinedname/type/) { get; } | Representa el tipo de revisión. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Obtiene la hoja de cálculo. (Heradado de [`Revision`](../revision/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDefinedNameDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Agregar un nombre definido al libro de trabajo
                int nameIndex = workbook.Worksheets.Names.Add("TestDefinedName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Modificar el nombre definido para crear una revisión
                definedName.RefersTo = "=Sheet1!$B$1";

                // Guardar el libro de trabajo para generar registros de revisión
                string filePath = "RevisionDefinedNameDemo.xlsx";
                workbook.Save(filePath);

                // Reabrir el libro de trabajo para acceder a la información de revisión
                Workbook revisionWorkbook = new Workbook(filePath);

                // Iterar a través de los registros de revisión para encontrar entradas de RevisionDefinedName
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;

                            // Mostrar las propiedades de RevisionDefinedName
                            Console.WriteLine($"Revision Type: {revisionDefinedName.Type}");
                            Console.WriteLine($"Defined Name Text: {revisionDefinedName.Text}");
                            Console.WriteLine($"Old Formula: {revisionDefinedName.OldFormula}");
                            Console.WriteLine($"New Formula: {revisionDefinedName.NewFormula}");
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

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


