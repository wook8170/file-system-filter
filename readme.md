# Windows File System Filter Driver Development Tutorial

## About

A simple Windows file system filter driver solution, created mainly for the demonstration and further customization purposes.

The main purpose when you develop a file system filter driver is to change file system behavior. It is called at each I/O operation and provides possibility to additionally process its parameters and change its results (�filter� this request).

File system filter driver development is used for context-based permission management, configuration change management, access management, continuous backup solutions, anti-malware solutions and many other applications.

Author: @SergiusTheBest

## Implementation

The code is written in C++. You will also need WDK/IFS kit to build the solution.
You can find a step-by-step file system filter driver tutorial with code samples as well as instructions on how to install/uninstall and start/stop this driver in the [detailed related article](https://www.apriorit.com/dev-blog/167-file-system-filter-driver).

## License

Licensed under the MIT license. � Apriorit.

## How to build

To build filter driver solution you need:
- Visual Studio 2019 16.4 or higher (with all SDK available in additional features);
- Windows 10 SDK 10.1.18362.1 or higher;
- WDK 10.1.18362.1 or higher;
- MSVC v142 C++ Spectre-Mitigation tools (via Visual Studio Installer -> Individual Components).

After installing all the necessary tools open FsFilter.sln file and build FsFilter project.
