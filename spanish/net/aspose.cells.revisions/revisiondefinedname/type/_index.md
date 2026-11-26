---
title: "RevisionDefinedName.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RevisionDefinedName. Representa el tipo de revisión"
type: docs
url: /es/net/aspose.cells.revisions/revisiondefinedname/type/
---
## RevisionDefinedName.Type property

Representa el tipo de revisión.

```csharp
public override RevisionType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionDefinedNamePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo y agregar un nombre definido
                Workbook wb = new Workbook();
                Worksheet ws = wb.Worksheets[0];

                int nameIdx = wb.Worksheets.Names.Add("DemoName");
                Name definedName = wb.Worksheets.Names[nameIdx];
                definedName.RefersTo = "=Sheet1!$A$1";

                // Cambiar el nombre definido para generar un registro de revisión
                definedName.RefersTo = "=Sheet1!$B$1";

                // Guardar el libro de trabajo para incrustar información de revisión
                string filePath = "RevisionDefinedName_TypeDemo.xlsx";
                wb.Save(filePath);

                // Re‑abrir el libro de trabajo para leer el registro de revisión
                Workbook revWb = new Workbook(filePath);

                // Iterar a través de las revisiones y mostrar el Type de cada entrada RevisionDefinedName
                foreach (RevisionLog log in revWb.Worksheets.RevisionLogs)
                {
                    foreach (Revision rev in log.Revisions)
                    {
                        if (rev.Type == RevisionType.DefinedName)
                        {
                            RevisionDefinedName rdn = (RevisionDefinedName)rev;
                            Console.WriteLine($"Revision Type: {rdn.Type}");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionDefinedName](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


