---
title: "NameCollection.Remove"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método NameCollection. Eliminar una matriz de nombres"
type: docs
url: /es/net/aspose.cells/namecollection/remove/
---
## Remove(string[]) {#remove_1}

Eliminar una matriz de nombres

```csharp
public void Remove(string[] names)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombres | String[] | El texto de los nombres. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodRemoveWithStringArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenga la NameCollection del libro de trabajo
            NameCollection names = workbook.Worksheets.Names;
            
            // Agregar algunos rangos con nombre para demostrar la eliminación
            names.Add("TestRange1");
            names.Add("TestRange2");
            names.Add("TestRange3");
            
            // Preparar la matriz de nombres a eliminar
            string[] namesToRemove = new string[] { "TestRange1", "TestRange3" };

            try
            {
                // Llamar al método Remove con el parámetro String[]
                names.Remove(namesToRemove);
                
                Console.WriteLine("Names removed successfully:");
                foreach (string name in namesToRemove)
                {
                    Console.WriteLine(name);
                }
                
                // Mostrar los nombres restantes
                Console.WriteLine("\nRemaining names in the collection:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("NameCollectionRemoveDemo.xlsx");
        }
    }
}
```

### Ver también

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove}

Eliminar el nombre.

```csharp
public void Remove(string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | String | El texto del nombre. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar un rango con nombre
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1", "B10");
            range.Name = "TestRange";
            
            // Mostrar recuento antes de la eliminación
            Console.WriteLine("Named ranges count before removal: " + workbook.Worksheets.Names.Count);
            
            // Eliminar el rango con nombre
            workbook.Worksheets.Names.Remove("TestRange");
            
            // Mostrar recuento después de la eliminación
            Console.WriteLine("Named ranges count after removal: " + workbook.Worksheets.Names.Count);
        }
    }
}
```

### Ver también

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


