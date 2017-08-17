# FiveM Config Reader
A simple c# config file reader for FiveM, which is designed to read config files such as (ini files), and load it in a way you can easily read it.

To use this with your own c# scripts; simply download ConfigReader.cs and add it to your project, you will then be able to reference it in your script like so:

using Config.Reader;
iniconfig config = new iniconfig("resourceName","file");

You will then be able to access the ini file's data using its methods, like so:

config.GetStringValue("section","key","fallback");

To correctly load resources you must first create the ini and add it to your __resource.lua file like so:
file 'fileName' 
