---
title: "RevisionRenameSheet.NewName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionRenameSheet. Obtiene el nuevo nombre de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.revisions/revisionrenamesheet/newname/
---
## RevisionRenameSheet.NewName property

Obtiene el nuevo nombre de la hoja de cálculo.

```csharp
public string NewName { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionRenameSheetPropertyNewNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y renombrarla para generar una revisión
            Worksheet sheet = workbook.Worksheets[0];
            string originalName = sheet.Name;
            string newName = "RenamedSheet";
            sheet.Name = newName;

            // Guardar en un flujo de memoria para generar revisiones
            System.IO.MemoryStream ms = new System.IO.MemoryStream();
            workbook.Save(ms, SaveFormat.Xlsx);

            // Reabrir el libro de trabajo para acceder a los registros de revisiones
            workbook = new Workbook(ms);
            
            // Verificar los registros de revisiones para la operación de renombrado
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.RenameSheet)
                    {
                        RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
                        Console.WriteLine("Sheet renamed from '{0}' to '{1}'", 
                            renameSheet.OldName, renameSheet.NewName);
                        
                        // Demostrar el uso de la propiedad NewName
                        if (renameSheet.NewName == newName)
                        {
                            Console.WriteLine("NewName property verification successful");
                        }
                    }
                }
            }
        }
    }
}
```

### Ver también

* class [RevisionRenameSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


