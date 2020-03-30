## How To Adjust Settings

[Go Back To Main Page](https://github.com/rufio-tf2/pg-config/#pg-starter-config)

### How To Open File For Editing

Don't use Wordpad, Microsoft Word, OpenOffice, LibreOffice, etc.

Windows comes with Notepad installed, so I'll use that for the example:

1. Navigate to `tf/custom/pg-config-master/cfg/custom.cfg`
1. Right-click on `custom.cfg`
1. Hover over "Open with..."
1. Find and select "Notepad" in the list of apps

**Make sure you save the file after you make changes.**

### How To Change Settings

In `custom.cfg`, find the "PG Settings" section near the top.

Say you want to turn gore on (blood and "gibs"). Change the line that says `goreOff` to instead say `goreOn`.

<table>
  <tr>
    <th>Remove <code>goreOff</code></th>
    <th>Add <code>goreOn</code></th>
  </tr>
  <tr>
    <td>
      <pre lang="diff">
    // PG Settings
    chatOff
    unbindChat
    voiceOff
-   goreOff
    spraysOff
          </pre>
    </td>
    <td>
      <pre lang="diff">
    // PG Settings
    chatOff
    unbindChat
    voiceOff
+   goreOn
    spraysOff
          </pre>
    </td>
  </tr>
</table>

**Save the file.** Now gore will be turned on after you restart TF2.

### Available Settings

- **`voiceOff`**/`voiceOn` -- Disable/Enable voice chat
- **`chatOff`**/`chatOn` -- Disable/Enable text chat
- **`unbindChat`**/`bindChat` -- Unbind/Bind default text and voice chat keys
- **`goreOff`**/`goreOn` -- Disable/Enable blood and gibs
- **`spraysOff`**/`spraysOn` -- Disable/Enable seeing player sprays

[Go Back To Main Page](https://github.com/rufio-tf2/pg-config/#pg-starter-config)
