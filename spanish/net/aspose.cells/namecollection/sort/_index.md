---
title: "NameCollection.Sort"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método NameCollection. Ordena los nombres definidos"
type: docs
url: /es/net/aspose.cells/namecollection/sort/
---
## NameCollection.Sort method

Ordena los nombres definidos.

```csharp
public void Sort()
```

### Observaciones

Si crea una gran cantidad de rangos con nombre en el archivo Excel, por favor llame a este método después de crear todos los rangos con nombre y antes de guardar

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodSortDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenga la NameCollection del libro de trabajo
            NameCollection names = workbook.Worksheets.Names;
            
            // Agregue algunos rangos con nombre para demostrar la ordenación
            names.Add("RangeC");
            names.Add("RangeA");
            names.Add("RangeB");
            
            try
            {
                // Mostrar nombres antes de ordenar
                Console.WriteLine("Names before sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
                
                // Llame al método Sort
                names.Sort();
                
                // Mostrar nombres después de ordenar
                Console.WriteLine("\nNames after sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Sort method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("NameCollectionSortDemo.xlsx");
        }
    }
}
```

### Ver también

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


