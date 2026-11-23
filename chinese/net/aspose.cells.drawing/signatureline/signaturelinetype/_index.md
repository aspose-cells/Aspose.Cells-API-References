---
title: "SignatureLine.SignatureLineType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SignatureLine 属性。获取或设置签名类型。Default 当默认值被设置时，相应的 ProviderId 值固定为 00000000000000000000000000000000。Stamp 当值为 Stamp 时，相应的 ProviderId 值通常为 000CD6A400000000C000000000000046。Custom 当值为 Custom 时，相应的 ProviderId 值通常需要用户设置。应从随提供程序附带的文档中获取。"
type: docs
url: /zh/net/aspose.cells.drawing/signatureline/signaturelinetype/
---
## SignatureLine.SignatureLineType property

获取或设置签名类型。Default - 当默认值被设置时，相应的 ProviderId 值固定为 {0000000000-0000-0000-0000-0000000000}。Stamp - 当值为 Stamp 时，相应的 ProviderId 值通常为 {000CD6A4-0000-0000-C000-000000000046}。Custom - 当值为 Custom 时，相应的 ProviderId 值通常需要用户设置。应从随提供程序附带的文档中获取。

```csharp
public SignatureType SignatureLineType { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLinePropertySignatureLineTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建签名行
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Developer";
            signatureLine.Email = "john@example.com";
            signatureLine.IsLine = true;
            signatureLine.AllowComments = true;
            signatureLine.ShowSignedDate = true;
            signatureLine.Instructions = "Please sign here";

            // 显示当前 SignatureLineType
            Console.WriteLine("Current SignatureLineType: " + signatureLine.SignatureLineType);

            // 将 SignatureLineType 设置为 Stamp
            signatureLine.SignatureLineType = SignatureType.Stamp;
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("ProviderId after Stamp type: " + signatureLine.ProviderId);

            // 通过将其添加到形状，将签名行添加到工作表
            Picture signaturePicture = worksheet.Shapes.AddSignatureLine(0, 0, signatureLine); // Changed to Picture type
            Console.WriteLine("Added signature line with index: " + signaturePicture.OriginalHeight);

            // 将 SignatureLineType 更改为 Custom，并使用自定义 ProviderId
            signatureLine.SignatureLineType = SignatureType.Custom;
            signatureLine.ProviderId = Guid.NewGuid();
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("Custom ProviderId: " + signatureLine.ProviderId);

            // 保存工作簿
            workbook.Save("SignatureLineTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [SignatureType](../../signaturetype/)
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


