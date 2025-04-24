---
author: ["ShenEn"]
title: "Test"
date: "2025-04-24"
description: "description"
summary: "summart"
tags: ["csharp", "markdown", "code","s7"]
categories: ["themes", "syntax"]
series: ["Themes Guide"]
ShowToc: true
TocOpen: true
social:
  fediverse_creator: "@adityatelange@mastodon.social"
---

### Code

```csharp {linenos=true}
Console.WriteLine("Start the simulated PLC server...");

var s7NetServer = new SiemensS7Server();
s7NetServer.ServerStart(102);

for (var index = 1; index < 273; index++)
{
    s7NetServer.AddDbBlock(index);
}

Console.ReadKey();
```
