---
title: "ExternalLinkCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ExternalLinkCollection. Elimina el enlace externo especificado del libro de trabajo"
type: docs
url: /es/net/aspose.cells/externallinkcollection/removeat/
---
## RemoveAt(int) {#removeat}

Elimina el enlace externo especificado del libro de trabajo.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | el índice del enlace externo a eliminar. |

### Observaciones

Al eliminar el enlace externo, todas las fórmulas que hacen referencia a él también se eliminarán porque las referencias se vuelven inválidas.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con enlaces externos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos enlaces externos de ejemplo
            worksheet.Cells["A1"].Formula = "='C:/ExternalFiles/File1.xlsx'!Sheet1!A1";
            worksheet.Cells["A2"].Formula = "='C:/ExternalFiles/File2.xlsx'!Sheet1!A1";
            worksheet.Cells["A3"].Formula = "='C:/ImportantFiles/File3.xlsx'!Sheet1!A1";

            // Obtener la colección de enlaces externos
            ExternalLinkCollection elc = workbook.Worksheets.ExternalLinks;
            Console.WriteLine("Initial external links count: " + elc.Count);

            // Eliminar los enlaces externos que no contengan "ImportantFiles" en su ruta
            for (int i = elc.Count - 1; i >= 0; i--)
            {
                if (!elc[i].DataSource.Contains("ImportantFiles"))
                {
                    elc.RemoveAt(i);
                }
            }

            Console.WriteLine("Remaining external links count: " + elc.Count);
            Console.WriteLine("Remaining external link path: " + elc[0].DataSource);
        }
    }
}
```

### Ver también

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, bool) {#removeat_1}

Elimina el enlace externo especificado del libro de trabajo.

```csharp
public void RemoveAt(int index, bool updateReferencesAsLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | el índice del enlace externo a eliminar. |
| updateReferencesAsLocal | Boolean | Indica si se actualizan todas las referencias del enlace externo dado a la referencia del propio libro de trabajo actual. Consulte [`Clear`](../clear/) para obtener más detalles sobre este parámetro. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodRemoveAtWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook wb = new Workbook();
            
            // Agregar algunos enlaces externos
            ExternalLinkCollection elc = wb.Worksheets.ExternalLinks;
            elc.Add("externallink1.xlam", new string[] { "externallink1.xlam" });
            elc.Add("externallink2.xlam", new string[] { "externallink2.xlam" });
            elc.Add("externallink3.xlam", new string[] { "externallink3.xlam" });
            elc.Add("externallink4.xlam", new string[] { "externallink4.xlam" });

            // Agregar algunas fórmulas que referencian estos enlaces externos
            Worksheet ws = wb.Worksheets[0];
            for (int i = 0; i < 4; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    ws.Cells[j, i].Formula = $"=externallink{i+1}.xlam!customfunc{j+1}()";
                }
            }

            Console.WriteLine($"Initial external links count: {elc.Count}");
            Console.WriteLine("Formulas before removal:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {ws.Cells[0, i].Formula}");
            }

            // Eliminar en el índice 1 con updateReferences=true
            elc.RemoveAt(1, true);
            
            Console.WriteLine($"\nAfter removing at index 1 (updateReferences=true):");
            Console.WriteLine($"External links count: {elc.Count}");
            Console.WriteLine("Updated formulas:");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {ws.Cells[0, i].Formula}");
            }

            // Eliminar en el índice 0 con updateReferences=false
            elc.RemoveAt(0, false);
            
            Console.WriteLine($"\nAfter removing at index 0 (updateReferences=false):");
            Console.WriteLine($"External links count: {elc.Count}");
            Console.WriteLine("Formulas (should be cleared where references were removed):");
            for (int i = 0; i < 2; i++)
            {
                Console.WriteLine($"Cell A{i+1}: Has formula? {ws.Cells[0, i].IsFormula}");
            }
        }
    }
}
```

### Ver también

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


