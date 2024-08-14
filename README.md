RUN: dotnet publish /t:PublishContainer Test/Test.csproj

```
> dotnet publish /t:PublishContainer Test/Test.csproj

  Determining projects to restore...
  All projects are up-to-date for restore.
  Test2 -> D:\private-github\DotnetContainerPublish8-0-400-Repro\Test2\bin\Release\net8.0\Test2.dll
  Test3 -> D:\private-github\DotnetContainerPublish8-0-400-Repro\Test3\bin\Release\net8.0\Test3.dll
  Test -> D:\private-github\DotnetContainerPublish8-0-400-Repro\Test\bin\Release\net8.0\Test.dll
  Test -> D:\private-github\DotnetContainerPublish8-0-400-Repro\Test\bin\Release\net8.0\publish\
MSBUILD : error MSB4166: Child node "2" exited prematurely. Shutting down. Diagnostic information may be found in files in "C:\Users\RemcovanOosterhout\AppData\Local\Temp\MSBuildTemp\" and
will be named MSBuild_*.failure.txt. This location can be changed by setting the MSBUILDDEBUGPATH environment variable to a different directory.
MSBUILD : error MSB4166: C:\Users\RemcovanOosterhout\AppData\Local\Temp\MSBuildTemp\MSBuild_pid-30864_86a9c20c09c04d99b1f1231a65f21341.failure.txt:
MSBUILD : error MSB4166: UNHANDLED EXCEPTIONS FROM PROCESS 30864:
MSBUILD : error MSB4166: =====================
MSBUILD : error MSB4166: 8/14/2024 10:10:31 AM
MSBUILD : error MSB4166: System.ArgumentNullException: Value cannot be null. (Parameter 'value')
MSBUILD : error MSB4166:    at System.ArgumentNullException.Throw(String paramName)
MSBUILD : error MSB4166:    at System.IO.BinaryWriter.Write(String value)
MSBUILD : error MSB4166:    at Microsoft.Build.Framework.TelemetryEventArgs.WriteToStream(BinaryWriter writer)
MSBUILD : error MSB4166:    at Microsoft.Build.Shared.LogMessagePacketBase.WriteToStream(ITranslator translator)
MSBUILD : error MSB4166:    at Microsoft.Build.BackEnd.NodeEndpointOutOfProcBase.RunReadLoop(Stream localReadPipe, Stream localWritePipe, ConcurrentQueue`1 localPacketQueue, AutoResetEvent
localPacketAvailable, AutoResetEvent localTerminatePacketPump)
MSBUILD : error MSB4166: ===================
MSBUILD : error MSB4166:
MSBUILD : error MSB4166:
```