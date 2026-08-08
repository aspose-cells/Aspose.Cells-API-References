---
title: "Metered.setMeteredKey"
linktitle: "setMeteredKey"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Sets metered public and private key."
type: docs
weight: 20
url: /nodejs/aspose.cells/metered/setmeteredkey/
---

## setMeteredKey(publicKey, privateKey)

Sets metered public and private key. If you purchase metered license, when start application, this API should be called, normally, this is enough. However, if always fail to upload consumption data and exceed 24 hours, the license will be set to evaluation status, to avoid such case, you should regularly check the license status, if it is evaluation status, call this API again.

| Parameter | Type | Description |
| --- | --- | --- |
| publicKey | String | public key |
| privateKey | String | private key |
