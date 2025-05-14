---
title: Metered.SetMeteredKey
second_title: Aspose.Cells for .NET API Reference
description: Metered method. Sets metered public and private key. If you purchase metered license when start application this API should be called normally this is enough. However if always fail to upload consumption data and exceed 24 hours the license will be set to evaluation status to avoid such case you should regularly check the license status if it is evaluation status call this API again
type: docs
url: /net/aspose.cells/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Sets metered public and private key. If you purchase metered license, when start application, this API should be called, normally, this is enough. However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | String | public key |
| privateKey | String | private key |

### Examples

```csharp
// Called: new Metered().SetMeteredKey("asposenet7c90badb00ba4f4bbd35634f4d481c14",
private void Metered_Method_SetMeteredKey(string plugin)
        {
            if (plugin == "Pdf")
            {
                new Metered().SetMeteredKey("asposenet83676f99cdbf40b5b2128dc29a243e46",
                    "vGQeiPLG9KJNGku8YOiDxvfouC5jtTmKfDiKU*ZX3ycAvQgYOvtN8jTjRqv2ulrU-hoMmcc*TmkKv5YzyaSvQk1Ubqx0nr2G1v0X4bZW6JuOzIpxoKytggsIDm3UG6OOz7KQTo2Q3vSfwQHbVjjqukgctHahWRcJQkrzHEl2jVt7rNWut1H48AWxjWIydG*Z2klUbToKWUXYG7LHnpG3Y3XVGUEtUyIEvP3UoUtmiOTcOJbjPAEFJSDZLPSDkCvMcHtyDiN3DG7daRw*sIrqBs4y21-0zBwH1vw26cTdYFqDD9Raxg7viV4EyTS0FFOUtLSeZfs9xzO3h8sLXl628A__");
                return;
            }
            if (plugin == "Image")
            {
                new Metered().SetMeteredKey("asposenet9fae554fd3404a3ba42636d8e96f99ef",
                    "iXJagUyG-*K4rmE-5gO3aquODsvlSShMAzWxoZp-M2pGMF7ng-iY17CSB4FMB42xGR*a0*V1jqnaz75g9EHhJV0lrB-GVFSYqUDndJNQCg6t7i8LJGhr*LRULtTFKzUfc-LWV*0kijQUV2hiYELaelvIjgHRrIqzy8QoGgrx12YF6S-3SKJpME*tL*kiWydRR-KV233gFZv436PV3n3g*QaSZ9PmILuQVqTPXnyU4JUNnBotQNXDg4fENGx1rnEV4QYpInS6urvr-UhIDaTR3hoiEK*KMZ5-x3QYcaRiECewQktRAZoApISnlx1MWt9Js8zGoZ1hId3*zGiNh5CruQ__");
                return;
            }
            if (plugin == "Spreadsheet")
            {
                //new Metered().SetMeteredKey("",
                //    "");
                return;
            }
            if (plugin == "Text")
            {
                new Metered().SetMeteredKey("asposenet99c76e3db0e04aeeb04b4023efc45b43",
                    "d0yR*oUBd*tVVaVFn5dOWMtGbjU0CLOqRHJal4TA-4vw7yJtKD3tJj6ReNlsMR2tdtFyGaS37tuWxxv-gNqfoZP3uGVmnoMdjlUpE04EUW6DxFchmL2SNWSLpi4HWEHlmagpIHkJlPUNMvU*VMnojoIonH59SLSzlH-zZF-f0HvMQx-JpfaneVpSPr9tbkXyRHTaIjnLu-KFmRcCnux6I1LyZRYRjesNRE7xrBEtFU-iWPo0sDBuehCl6wwlLVkZZI-2DYAIU-42g51d-20afjZPVgQw0DHeZuScOeRVm5Pt8rAaqywfFXwdnoQdCYAatPrb38T-ktsEpP9LPFQTAQ__");
                return;
            }
            if (plugin == "Json")
            {
                new Metered().SetMeteredKey("asposenet7c90badb00ba4f4bbd35634f4d481c14",
                    "FBJnGi61yW8meqVfugVpqX5WXyBIgDOp-XaEV5MjzuABC9OKu6SwMP00KWZo8ULVfvkYPG4thnNerNPvvRohz1hAMjG9SkQ4akclON6VqBdXuxbasF1aXwShbIBNTA7Ac*3OnFxDo4jcvg0XyTSyQjA*vxhq*0YEr2MgedtncGUiCyC7o775f7uXusxe*UWVDdI*qNzEdSU*f7Sl6a9qiDBAA*q2OrXbd9jOAgiP1TiAq6vluG7vqK-dKZlTOmL*A-Uo0rxU73ZjtYW*TLZAW2jTbzVIOHyws3l6DF5G98ayvKt1iye5ce4HNkvxwk3*uNyMd-JQeGz64hQpjU5Cdw__");
                return;
            }
            if (plugin == "Html")
            {
                new Metered().SetMeteredKey("asposenet37bfe1d90b4e4e6ca0e7e9231e1d86ab",
                    "MG7sb2rg3pNxCzMAZTjIc2eRmGgb*C-MrVZyjx-RkjYw-i*aI*pukSHcdtOO6hKWj6ItWIoTatOHhM5AAMelp4kklntnGxJ41s*BFupZ*7FvLioxKrPubwzQBgZRlTC7Tz9UmPKrAM*Lwf3E*kiPTX3ugEk5Chi*Hrd8tfF1GvaiCapp2QnRPG7bXzAQNnRKd2fB*YCDg9iilvcy9SH5OcrtbCG8Oq6ELC3jhC5wRbqBzTcYMnwDGN8TtgRbHO0VxXzvQ9H2MHGVlKXSuN6z41Os4WTzmLjs8YXbNqNXJDRcYMrDqSehg*uhPRPpHdqIPfD1AZsJlsf6CZ1I*wDtWA__");
                return;
            }
            if (plugin == "Split")
            {
                //new Metered().SetMeteredKey("",
                //    "");
                return;
            }
            if (plugin == "Merge")
            {
                //new Metered().SetMeteredKey("",
                //    "");
                return;
            }
            if (plugin == "Lock")
            {
                new Metered().SetMeteredKey("asposenetdf327abc886c43f5b0fb604a004f166f",
                    "foDbeMYLhFYNxgKQa5B2uJh5w6DIfskvxkQkrhKdlhQTn8Z4sesz1B*tpCUJliOv2eUy5tMFkjTrhtXFFVHz2OzIzd-fkDZ3yUYzXCAHnmXz6yktYwsFGkYF9ZGP7DWXY5FU884sR9ND605fH9OE2NMbq*vFYLWy8FThAXpaGc3hmBFaaXFv4jO8lowr8lQk9ofR4rY8fAKi*L7G8t1MdL0smXOiP2Ji8TRza21FQC*7juZLGOCokmEnSbanS9MimMGfq6lKLb80kXSIsoI8V-xt7iGobdPz8w0qhddF2aDEoiSnRx7YaSy7dgxeIh414vHR1572yOFK5GuHQpYaUA__");
                return;
            }
            if (plugin == "Unlock")
            {
                //new Metered().SetMeteredKey("",
                //    "");
                return;
            }
            Assert.Fail("Unknown plugin for license: " + plugin);
        }
```

### See Also

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


