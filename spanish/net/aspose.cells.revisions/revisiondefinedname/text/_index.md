---
title: "RevisionDefinedName.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionDefinedName. Obtiene el texto del nombre definido"
type: docs
url: /es/net/aspose.cells.revisions/revisiondefinedname/text/
---
## RevisionDefinedName.Text property

Obtiene el texto del nombre definido.

```csharp
public string Text { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionDefinedNamePropertyTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un nombre definido
            int index = workbook.Worksheets.Names.Add("TestName");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1";
            
            // Modificar el nombre definido para generar una revisión
            name.RefersTo = "=Sheet1!$B$1";
            
            // Guardar en archivo para generar revisiones
            workbook.Save("RevisionDefinedName.xlsx");
            
            // Reabrir el archivo para leer revisiones
            Workbook revisionWorkbook = new Workbook("RevisionDefinedName.xlsx");
            
            // Verificar revisiones
            foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
            {
                foreach (Revision rv in log.Revisions)
                {
                    if (rv.Type == RevisionType.DefinedName)
                    {
                        RevisionDefinedName rdn = (RevisionDefinedName)rv;
                        Console.WriteLine("Defined Name Text: " + rdn.Text);
                        Console.WriteLine("Old Formula: " + rdn.OldFormula);
                        Console.WriteLine("New Formula: " + rdn.NewFormula);
                    }
                }
            }
        }
    }
}
```

### Ver también

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


