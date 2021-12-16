# Durable Function

A sample durable function

## Dev Container

- Ubuntu 20.04
- DotNet 6
- Functions Runtime 4
- Extensions
    - C#
    - Azure Functions
    - Azure CLI
    - Azurite

## Durable Functions Code

- C#
- Standard orchestrator sample
- Using Azurite for storage emulation

### Sample Output

Using the Dev Container, start Azurite from the taskbar (getting it running on open seems to be a pain), then start debugging.
You should get a URL, and this sort of output;

```text
Azure Functions Core Tools
Core Tools Version:       4.0.3971 Commit hash: d0775d487c93ebd49e9c1166d5c3c01f3c76eaaf  (64-bit)
Function Runtime Version: 4.0.1.16815

[2021-12-16T17:21:52.645Z] Found /workspaces/durablefunction/durablefunction.csproj. Using for user secrets file configuration.

Functions:

        OrchFunction_HttpStart: [GET,POST] http://localhost:7071/api/OrchFunction_HttpStart

        OrchFunction: orchestrationTrigger

        OrchFunction_Hello: activityTrigger

For detailed output, run func with --verbose flag.
[2021-12-16T17:22:00.886Z] Host lock lease acquired by instance ID '000000000000000000000000706166F2'.
[2021-12-16T17:22:22.849Z] Executing 'OrchFunction_HttpStart' (Reason='This function was programmatically called via the host APIs.', Id=4413460e-513e-43ae-bfb1-a6b8c92e9487)
[2021-12-16T17:22:23.008Z] Started orchestration with ID = '7fb920eb671740e685ccfb303be1b293'.
[2021-12-16T17:22:23.135Z] Executed 'OrchFunction_HttpStart' (Succeeded, Id=4413460e-513e-43ae-bfb1-a6b8c92e9487, Duration=307ms)
[2021-12-16T17:22:23.292Z] Executing 'OrchFunction' (Reason='(null)', Id=a8e06666-0494-417f-b808-e5cfb8e80e27)
[2021-12-16T17:22:23.312Z] Executed 'OrchFunction' (Succeeded, Id=a8e06666-0494-417f-b808-e5cfb8e80e27, Duration=21ms)
[2021-12-16T17:22:23.388Z] Executing 'OrchFunction_Hello' (Reason='(null)', Id=f2d74fc4-224e-444f-8564-7332a8889099)
[2021-12-16T17:22:23.391Z] Saying hello to Tokyo.
[2021-12-16T17:22:23.392Z] Executed 'OrchFunction_Hello' (Succeeded, Id=f2d74fc4-224e-444f-8564-7332a8889099, Duration=6ms)
[2021-12-16T17:22:23.484Z] Executing 'OrchFunction' (Reason='(null)', Id=7f19d6ba-19ae-45ad-9e3b-2f1a0c5d8fef)
[2021-12-16T17:22:23.490Z] Executed 'OrchFunction' (Succeeded, Id=7f19d6ba-19ae-45ad-9e3b-2f1a0c5d8fef, Duration=5ms)
[2021-12-16T17:22:23.534Z] Executing 'OrchFunction_Hello' (Reason='(null)', Id=ca56be0b-9d23-4d4c-8bbd-41e17b6eae53)
[2021-12-16T17:22:23.558Z] Saying hello to Seattle.
[2021-12-16T17:22:23.559Z] Executed 'OrchFunction_Hello' (Succeeded, Id=ca56be0b-9d23-4d4c-8bbd-41e17b6eae53, Duration=45ms)
[2021-12-16T17:22:23.631Z] Executing 'OrchFunction' (Reason='(null)', Id=7c6b2f71-f1fd-449b-9622-2f4ece10c53e)
[2021-12-16T17:22:23.634Z] Executed 'OrchFunction' (Succeeded, Id=7c6b2f71-f1fd-449b-9622-2f4ece10c53e, Duration=3ms)
[2021-12-16T17:22:23.680Z] Executing 'OrchFunction_Hello' (Reason='(null)', Id=06e8bd28-4408-4bf8-a617-c77e8e5dded7)
[2021-12-16T17:22:23.702Z] Saying hello to London.
[2021-12-16T17:22:23.728Z] Executed 'OrchFunction_Hello' (Succeeded, Id=06e8bd28-4408-4bf8-a617-c77e8e5dded7, Duration=48ms)
[2021-12-16T17:22:23.907Z] Executing 'OrchFunction' (Reason='(null)', Id=c2f9d0c4-ba12-4d2f-a061-2806b6b9beac)
[2021-12-16T17:22:23.916Z] Executed 'OrchFunction' (Succeeded, Id=c2f9d0c4-ba12-4d2f-a061-2806b6b9beac, Duration=8ms)
```