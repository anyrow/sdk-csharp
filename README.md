# Anyrow C# SDK

[![MIT License](https://img.shields.io/badge/license-MIT-blue)](./LICENSE)

C# client for the [Anyrow](https://anyrow.ai) extraction API, generated from its [OpenAPI spec](https://github.com/anyrow/openapi). .NET 10, trimming- and AOT-safe, no dependencies.

## Install

```bash
dotnet add package Anyrow.Sdk
```

## Use

```csharp
using System;
using Anyrow.Sdk;

using var anyrow = new AnyrowClient(new ClientConfig
{
    BaseUrl = "https://api.anyrow.ai",
    BearerToken = Environment.GetEnvironmentVariable("ANYROW_API_KEY"),
});
```

Every API operation is a method on `AnyrowClient`; request and response types live in `Anyrow.Sdk`. See the [API reference](https://anyrow.ai/docs) for what each one does.

## Other languages

[TypeScript](https://github.com/anyrow/sdk-typescript) · [Python](https://github.com/anyrow/sdk-python) · [Go](https://github.com/anyrow/sdk-go) · [Rust](https://github.com/anyrow/sdk-rust) · [Java](https://github.com/anyrow/sdk-java) · [CLI](https://github.com/anyrow/cli)
