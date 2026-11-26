---
title: "RevisionDefinedName.OldFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionDefinedName. Obtiene la fórmula anterior"
type: docs
url: /es/net/aspose.cells.revisions/revisiondefinedname/oldformula/
---
## RevisionDefinedName.OldFormula property

Obtiene la fórmula anterior.

```csharp
public string OldFormula { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionDefinedNamePropertyOldFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Agregar un nombre definido para generar historial de revisiones
                int nameIndex = workbook.Worksheets.Names.Add("SampleName");
                Name definedName = workbook.Worksheets.Names[nameIndex];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Modificar el nombre definido para crear una revisión
                definedName.RefersTo = "=Sheet1!$B$1";

                // Guardar el libro de trabajo para conservar revisiones
                string filePath = "OldFormulaDemo.xlsx";
                workbook.Save(filePath);

                // Reabrir el libro de trabajo para acceder a los registros de revisiones
                Workbook revisionWorkbook = new Workbook(filePath);

                // Iterar a través de los registros de revisión para encontrar revisiones de nombres definidos
                foreach (RevisionLog log in revisionWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName revisionDefinedName = (RevisionDefinedName)revision;
                            Console.WriteLine("Defined Name Text: " + revisionDefinedName.Text);
                            Console.WriteLine("Old Formula: " + revisionDefinedName.OldFormula);
                            Console.WriteLine("New Formula: " + revisionDefinedName.NewFormula);
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

* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


