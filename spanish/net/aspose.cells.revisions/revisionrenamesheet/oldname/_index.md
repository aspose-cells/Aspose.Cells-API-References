---
title: "RevisionRenameSheet.OldName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionRenameSheet. Obtiene el nombre antiguo de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.revisions/revisionrenamesheet/oldname/
---
## RevisionRenameSheet.OldName property

Obtiene el nombre antiguo de la hoja de cálculo.

```csharp
public string OldName { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionRenameSheetPropertyOldNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y renombrarla para generar una revisión
            Worksheet sheet = workbook.Worksheets[0];
            string originalName = sheet.Name;
            sheet.Name = "RenamedSheet";

            // Accede a los registros de revisiones
            foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.RenameSheet)
                    {
                        RevisionRenameSheet rsnm = (RevisionRenameSheet)rv;
                        Console.WriteLine("Sheet renamed from: {0} to: {1}", rsnm.OldName, rsnm.NewName);
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


