---
title: "RevisionDefinedName.NewFormula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionDefinedName. Obtiene la fórmula"
type: docs
url: /es/net/aspose.cells.revisions/revisiondefinedname/newformula/
---
## RevisionDefinedName.NewFormula property

Obtiene la fórmula.

```csharp
public string NewFormula { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionDefinedNamePropertyNewFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo y agregar algunos datos
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].Value = "Initial";

                // Agrega un nombre definido que apunta a A1
                int nameIdx = workbook.Worksheets.Names.Add("DemoName");
                Name definedName = workbook.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Cambiar el nombre definido para generar una revisión (ahora apunta a B1)
                definedName.RefersTo = "=Sheet1!$B$1";

                // Guardar el libro de trabajo para incrustar información de revisión
                string fileName = "RevisionDefinedName_NewFormulaDemo.xlsx";
                workbook.Save(fileName);

                // Reabrir el libro de trabajo para leer los registros de revisión
                Workbook revWorkbook = new Workbook(fileName);

                // Iterar a través de las revisiones y mostrar NewFormula
                foreach (RevisionLog log in revWorkbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rev in log.Revisions)
                    {
                        if (rev.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName rdn = (RevisionDefinedName)rev;
                            Console.WriteLine($"Defined Name Text: {rdn.Text}");
                            Console.WriteLine($"Old Formula: {rdn.OldFormula}");
                            Console.WriteLine($"New Formula: {rdn.NewFormula}");
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


