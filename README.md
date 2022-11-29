# how to convert form chd to 5keys bms

こんにちは。

## prepare to convert

1. download Scharfrichter from [SaxxonPike/scharfrichter: A library and toolset designed for rhythm games.](https://github.com/SaxxonPike/scharfrichter)
1. download chdman from [Releases · mamedev/mame](https://github.com/mamedev/mame/releases/)
   - `chdman.exe`

## convert

1. chd to raw
   - `chdman.exe extracthd -i input.chd -o output.raw`
1. build `DJMainExtract`
   1. open Scharfrichter.sln 
   1. change `Solution Configurations` to `Release`
   1. build solution `ctrl + shift + b`
      - `.\scharfrichter-master\DJMainExtract\bin\Release\DJMainExtract.exe`
  
        ```sh
        $ tree .
        .
        ├── ConvertHelper.dll
        ├── DJMainExtract.exe
        ├── NAudio.dll
        ├── Scharfrichter.Codec.dll
        └── Scharfrichter.Common.dll
        ```

1. run the command `.\scharfrichter-master\DJMainExtract\bin\Release\DJMainExtract.exe output.raw`
1. wait for a bit!!!!!!!!!!!!

## \[PS] built DJMainExtract.exe

download Scharfrichter from [Releases · SaxxonPike/scharfrichter](https://github.com/SaxxonPike/scharfrichter/releases)
