# Brackets Name-A-Project
Extension to enable personalized, per-project nicknames for projects.


![Settings menu](/images/settings-menu.png)

## Usage
### Configuring a project name
1. Open File -> Project name
2. Change the name and background color (hex, hsl, rgba or name) for your project
3. Press "Done"

### Resetting a name
1. Open File -> Project name
2. Leave the Project Name and Background color fields empty
3. Press "Done"

![Dropdown menu](/images/dropdown.png)

## Preferences

Following configuration options are available (under `petetnt.brackets-name-a-project`):

### defaultScope (String) 
> Default: `user` - By default the extension saves the project preferences to the global preferences file `brackets.json`. Changing this to `project` makes the extension save the values to project-level `.brackets.json`.

### namedProjects {Object}
> Object that consists of objects. The key is the full path to project, and the value for that key is an combination of _parentPath, _name (original name), name (current name) and background color. Automatically created by the dialog.

Example:

``` json
    "petetnt.brackets-name-a-project.namedProjects": {
        "C:/Users/Pete/AppData/Roaming/Brackets/extensions/user/petetnt.brackets-name-a-project/": {
            "_parentPath": "C:/Users/Pete/AppData/Roaming/Brackets/extensions/user/petetnt.brackets-name-a-project/",
            "_name": "petetnt.brackets-name-a-project",
            "name": "Name A Project Extension",
            "bgColor": "blue"
        }
    }
```

## Licence 
MIT

## Contributions
Contributions are welcome! Just open a new issue and/or send a pull request.