---
title: "XmlMap.DataBinding"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlMap. Obtiene un XmlDataBinding de este mapa"
type: docs
url: /es/net/aspose.cells/xmlmap/databinding/
---
## XmlMap.DataBinding property

Obtiene un [`XmlDataBinding`](../../xmldatabinding/) de este mapa.

```csharp
public XmlDataBinding DataBinding { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyDataBindingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar mapas XML de ejemplo
            string url1 = "https://example.com/data1.xml";
            string url2 = "https://example.com/data2.xml";
            
            // Agregar el primer mapa XML
            int mapIndex1 = workbook.Worksheets.XmlMaps.Add(url1);
            XmlMap map1 = workbook.Worksheets.XmlMaps[mapIndex1];
            
            // Agregar el segundo mapa XML
            int mapIndex2 = workbook.Worksheets.XmlMaps.Add(url2);
            XmlMap map2 = workbook.Worksheets.XmlMaps[mapIndex2];
            
            // Demostrar el uso de la propiedad DataBinding
            Console.WriteLine("First XML Map:");
            Console.WriteLine("Name: " + map1.Name);
            Console.WriteLine("Root Element: " + map1.RootElementName);
            Console.WriteLine("Data Binding URL: " + map1.DataBinding.Url);
            
            Console.WriteLine("\nSecond XML Map:");
            Console.WriteLine("Name: " + map2.Name);
            Console.WriteLine("Root Element: " + map2.RootElementName);
            Console.WriteLine("Data Binding URL: " + map2.DataBinding.Url);
            
            // Guarda el libro de trabajo
            workbook.Save("XmlMapDataBindingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [XmlDataBinding](../../xmldatabinding/)
* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


