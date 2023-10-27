# Localization Pack for Device Monitoring Studio

This repository hosts a community-based development page of free localization pack for [Device Monitoring Studio](//www.hhdsoftware.com/device-monitoring-studio) product from HHD Software Ltd.

Please browse our [Wiki](https://github.com/hhd-software/dms-localization-pack/wiki) for detailed instructions on using this repository and localization utility.

## Localization Utility System Requirements

* Operating system: Windows 7 or later (both 32 and 64 bit supported).
* .NET 4.8 Framework

## Finished Language Packs

Complete language packs are available directly in Device Monitoring Studio. Go to the **Tools » Settings » Languages** tab to see the list of published language packs and to download them.

Currently, the following language packs are complete for latest version of Device Monitoring Studio:


## Manually Building Language Packs

You can manually build non-complete language pack and use it in Device Monitoring Studio. Follow this procedure:

1. Install Git client.
2. Execute a Clone command for the following repository:

   ```
   git clone https://github.com/hhd-software/dms-localization-pack.git
   ```

3. Switch to your language's branch.
4. Run the supplied `langtool.exe` utility (located at the root of the repository) and open the `studio.xml` project file.
5. Execute the **File » Compile…** command and select the language you want to compile.
6. Make sure you have Device Monitoring Studio installed. Compile the Language Pack.
7. Run Device Monitoring Studio and select the language pack in corresponding box on the toolbar.

## Using Authoring Mode

Device Monitoring Studio may be launched in so-called "authoring" mode that will allow direct editing of most strings that can be localized. As a result, a *corrections* file is produced when the application is closed. This *corrections* file may be imported into the language pack editor.

To start Device Monitoring Studio in authoring mode, use the following command line:

```PowerShell
Studio.exe /authoring <path-to-corrections-file>
```

Where `<path-to-corrections-file>` should be replaced with a full path of the corrections file. Device Monitoring Studio adds the current date and time and `.xml` file extension to the end of the path. The file is created when the editor is closed.

### String Editing

To edit a title of a window, hold `Ctrl` and `Shift` keys and click on a window title. To edit a text label, a button, a checkbox or a radio button, hold `Ctrl` and `Shift` keys and click on a control. After finishing editing, press the `Enter` key. For multi-line controls, press `Ctrl+Enter`. Press `Esc` to discard your changes.

Please note that not all strings can be localized using authoring mode.

## Acknowledgements

