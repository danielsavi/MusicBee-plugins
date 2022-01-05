# MusicBee-plugins

:file_folder: SetSlackStatus-binaries - Musibee **SetSlackStatus** plugin

:file_folder: CSharpDll - [My updated version of C# Source 3.1](https://getmusicbee.com/help/api/)

What's new? Tested under Win11 x64

* Visual Studio 2019
* Minimum .NET 4.5
* C# 9.0 - switch pattern matching

```csharp
            public MusicBeeVersion MusicBeeVersion
            {
                get
                {
                    var version = ApiRevision switch
                    {
                        <= 25 => MusicBeeVersion.v2_0,
                        <= 31 => MusicBeeVersion.v2_1,
                        <= 33 => MusicBeeVersion.v2_2,
                        <= 38 => MusicBeeVersion.v2_3,
                        <= 43 => MusicBeeVersion.v2_4,
                        <= 47 => MusicBeeVersion.v2_5,
                        <= 48 => MusicBeeVersion.v3_0,
                        _     => MusicBeeVersion.v3_1
                    };
                    return version;
                }
            }
```