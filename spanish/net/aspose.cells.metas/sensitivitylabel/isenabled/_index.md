---
title: "SensitivityLabel.IsEnabled"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SensitivityLabel. Indica si la etiqueta de sensibilidad está habilitada"
type: docs
url: /es/net/aspose.cells.metas/sensitivitylabel/isenabled/
---
## SensitivityLabel.IsEnabled property

Indica si la etiqueta de sensibilidad está habilitada

```csharp
public bool IsEnabled { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIsEnabledDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Crear una instancia de etiqueta de sensibilidad
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Establezca las propiedades iniciales
                label.Id = "CONFIDENTIAL_001";
                
                // Demuestre la obtención del valor inicial de IsEnabled
                Console.WriteLine("Initial IsEnabled value: " + label.IsEnabled);
                
                // Establezca IsEnabled a true y muestre el cambio
                label.IsEnabled = true;
                Console.WriteLine("After enabling: " + label.IsEnabled);
                
                // Cambie el valor para demostrar que es de lectura y escritura
                label.IsEnabled = false;
                Console.WriteLine("After disabling: " + label.IsEnabled);
                
                // Guarda el libro de trabajo
                workbook.Save("IsEnabledDemo.xlsx");
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


