# Cross Platform Disk Test (CPDT)

Measuring storage performance (SSD, HDD, USB Flash etc.) and RAM speed across Windows, macOS and Android devices. Random and sequential throughput (read/write operations) is calculated in MB/s and can be compared in consistent and reliable manner between mobile and desktop platforms and devices.

![UI](https://raw.githubusercontent.com/maxim-saplin/CrossPlatformDiskTest/master/Img%203.png)

## Download & Try

- Windows (x86 and x64) and .NET Framework 4.8
  - https://github.com/maxim-saplin/CrossPlatformDiskTest/releases/download/2.3.3WPF/CPDT.zip

- macOS 10.13+
  - https://github.com/maxim-saplin/CrossPlatformDiskTest/releases/download/2.3.3/CPDT.app.zip

- Android 4.4+ 
  - Play Market: https://play.google.com/store/apps/details?id=com.Saplin.CPDT
  - APK: https://github.com/maxim-saplin/CrossPlatformDiskTest/releases/download/2.4.0/com.Saplin.CPDT.apk
  
- Linux Console App
  - GitHub repo: https://github.com/maxim-saplin/NetCoreStorageSpeedTest/

## Benchmark chart

https://maxim-saplin.github.io/cpdt_results/

![Results](https://raw.githubusercontent.com/maxim-saplin/CrossPlatformDiskTest/master/Results.jpg)

## How it works

The tests measure time it takes to read/write each block (RAM -> Disk, Disk -> RAM, RAM ->), let you choose read/write modes (e.g. turning on/off write buffering and file cache in memory), conduct series operations in sequential and random manner and show the average throughput (total traffic over total time) in MB/s for each test. The tests let you benchmark how same storage operations (FileStream.Write and FileStrem.Read) are handled by different OS across different devices and compare the results.
CPDT is single-threaded, no IO queues or parallel execution of reads/writes.

![Concept](https://raw.githubusercontent.com/maxim-saplin/CrossPlatformDiskTest/master/EnBlack.png)

## Technology

Xamarin.Forms, .NET Framework and Xamarin.WPF on Windows, Mono and Xamarin.Mac on macOS, Mono and Xamarin.Android on Android. Quite a few custom controls (Stack and Grid repeaters, clickable label) and renderers (changing mouse cursor when hovering over button and label on desktop)
