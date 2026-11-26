---
title: "SensitivityLabel.ContentMarkType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SensitivityLabel. Obtiene y establece los tipos de marcado de contenido que deben aplicarse a un archivo"
type: docs
url: /es/net/aspose.cells.metas/sensitivitylabel/contentmarktype/
---
## SensitivityLabel.ContentMarkType property

Obtiene y establece los tipos de marcado de contenido que deben aplicarse a un archivo.

```csharp
public SensitivityLabelMarkType ContentMarkType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyContentMarkTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Crear una instancia de etiqueta de sensibilidad
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Establecer propiedades básicas
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // Demostrar la propiedad ContentMarkType (lectura-escritura)
                Console.WriteLine("Initial ContentMarkType: " + label.ContentMarkType);
                
                // Establecer diferentes tipos de marcado de contenido
                label.ContentMarkType = SensitivityLabelMarkType.Header;
                Console.WriteLine("After setting Header: " + label.ContentMarkType);
                
                label.ContentMarkType = SensitivityLabelMarkType.Watermark;
                Console.WriteLine("After setting Watermark: " + label.ContentMarkType);
                
                // Mostrar el uso de banderas combinadas
                label.ContentMarkType = SensitivityLabelMarkType.Header | SensitivityLabelMarkType.Footer;
                Console.WriteLine("Combined Header+Footer: " + label.ContentMarkType);
                
                // Guarda el libro de trabajo
                workbook.Save("ContentMarkTypeDemo.xlsx");
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

* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


