---
title: "SensitivityLabel.Id"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SensitivityLabel. Obtiene y establece el id de la etiqueta de sensibilidad"
type: docs
url: /es/net/aspose.cells.metas/sensitivitylabel/id/
---
## SensitivityLabel.Id property

Obtiene y establece el id de la etiqueta de sensibilidad.

```csharp
public string Id { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Crear una instancia de etiqueta de sensibilidad
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Demostrar la configuración y obtención de la propiedad Id
                string testId = "CONFIDENTIAL_001";
                label.Id = testId;
                
                // Mostrar el valor del Id
                Console.WriteLine("Sensitivity Label Id: " + label.Id);
                
                // Cambie el valor Id para demostrar que es de lectura y escritura
                label.Id = "INTERNAL_USE_ONLY";
                Console.WriteLine("Updated Sensitivity Label Id: " + label.Id);
                
                // Muestre cómo la propiedad afecta a otras operaciones
                label.IsEnabled = true;
                Console.WriteLine($"Label {label.Id} is enabled: {label.IsEnabled}");
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

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


