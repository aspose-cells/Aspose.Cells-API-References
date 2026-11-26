---
title: "SensitivityLabel.AssignmentType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SensitivityLabel. Obtiene y establece el método de asignación para la etiqueta de sensibilidad"
type: docs
url: /es/net/aspose.cells.metas/sensitivitylabel/assignmenttype/
---
## SensitivityLabel.AssignmentType property

Obtiene y establece el método de asignación para la etiqueta de sensibilidad.

```csharp
public SensitivityLabelAssignmentType AssignmentType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyAssignmentTypeDemo
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
                
                // Demuestre la obtención del valor inicial de AssignmentType
                Console.WriteLine("Initial AssignmentType: " + label.AssignmentType);
                
                // Establezca AssignmentType a Privileged y muestre el cambio
                label.AssignmentType = SensitivityLabelAssignmentType.Privileged;
                Console.WriteLine("After setting Privileged: " + label.AssignmentType);
                
                // Cambie de nuevo a Standard para demostrar que es de lectura‑escritura
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                Console.WriteLine("After setting Standard: " + label.AssignmentType);
                
                // Guarda el libro de trabajo
                workbook.Save("AssignmentTypeDemo.xlsx");
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

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


