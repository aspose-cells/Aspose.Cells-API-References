---
title: "SensitivityLabel.IsRemoved"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SensitivityLabel. Indica si la etiqueta de sensibilidad fue eliminada"
type: docs
url: /es/net/aspose.cells.metas/sensitivitylabel/isremoved/
---
## SensitivityLabel.IsRemoved property

Indica si la etiqueta de sensibilidad fue eliminada.

```csharp
public bool IsRemoved { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIsRemovedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Cree una instancia de etiqueta de sensibilidad mediante reflexión
                // ya que la instanciación directa no está disponible
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // Establezca las propiedades requeridas
                label.Id = "SENSITIVE_DATA";
                label.IsEnabled = true;
                label.IsRemoved = false;
                
                // Muestre el valor inicial de IsRemoved
                Console.WriteLine("Initial IsRemoved value: " + label.IsRemoved);
                
                // Demuestre la configuración de la propiedad IsRemoved (ya que es de lectura y escritura)
                label.IsRemoved = true;
                Console.WriteLine("After setting IsRemoved: " + label.IsRemoved);
                
                // Cambie el valor de nuevo para mostrar que puede modificarse
                label.IsRemoved = false;
                Console.WriteLine("Final IsRemoved value: " + label.IsRemoved);
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


