# compbiz-plugin-settings
Bash script to easily modify Compbiz plugin settings for current profile.

## Status
Working but ugly.  Terminology may be incorrect.  This was written as a necessity for enabling a single plugin within my [dotfiles](https://github.com/FredLackey/dotfiles) and while having zero knowledge of Combpiz.

## Example Usage
For my purpose, I needed the ability to enable two settings when setting up my Ubuntu and Linux Mint workstations.

**Step 1: Enable the Plugin**
<pre>
enable_compiz_plugin put
</pre>
**Step 2: Apply the Settings**
<pre>
set_compiz_plugin_setting put put-next-output-key '<Shift><Alt>Right'

set_compiz_plugin_setting put put-prev-output-key '<Shift><Alt>Left'
</pre>

## Available Commands
Although I only needed the two commands, above, there are several more that you may find helpful:

<pre>
get_compiz_available_plugins
print_compiz_available_plugins
is_compiz_plugin_available
get_compiz_profile_name
get_compiz_profile_path
get_compiz_active_plugins
print_compiz_active_plugins
is_compiz_plugin_active
get_compiz_inactive_plugins
get_compiz_plugin_status
enable_compiz_plugin
disable_compiz_plugin
get_compiz_plugin_default_settings
get_compiz_plugin_active_settings
get_compiz_plugin_setting
set_compiz_plugin_setting
</pre>

## Statuses
The following three statuses are used when describing a plugin (all three based on the verbiage used by Compbiz):

#### Active
The plugin is installed and *is* active.

#### Available
The plugin is installed but *may or may not* be active.

#### Inactive
The plugin is installed but *is not* active.

## Profiles

#### Current
The profile your computer is currently using.

#### Default
The profile created by the configuration backend.


## Reference
This script was created based on the knowledge obtained from the Compbiz Configuration section of the [Arch Linux wiki](https://wiki.archlinux.org/index.php/Compiz_configuration).  I did try to contact the Compbiz authors directly but never received a response.

## Contact
Please feel free to contact me with any questions or comments:

Fred Lackey  
[fred.lackey@gmail.com](mailto:fred.lackey@gmail.com)  
[www.fredlackey.com](http://www.fredlackey.com)  

