Laravel 5 Artisan commands
===============

Fork of Sublime Text plugin for Laravel 4 Artisan commands

This plugin allows you the run the normal Artisan CLI using the Sublime Text interface, without having to open and use the command line.

Several of the commands, such as `Laravel Artisan: Make: Migration Schema` require `laracasts/generators` to be installed, as the associated commands are not native to Laravel (yet).

### Available commands:

##### Laravel Artisan
- `Laravel Artisan: Changes`
- `Laravel Artisan: Clear Compiled`
- `Laravel Artisan: Down`
- `Laravel Artisan: Dump Autoload`
- `Laravel Artisan: Help`
- `Laravel Artisan: List`
- `Laravel Artisan: Migrate`
- `Laravel Artisan: Optimize`
- `Laravel Artisan: Route`
- `Laravel Artisan: Serve`
- `Laravel Artisan: Up`
- `Laravel Artisan: Workbench`
- `Laravel Artisan: Asset: Publish`
- `Laravel Artisan: Auth: Reminders`
- `Laravel Artisan: Cache: Clear`
- `Laravel Artisan: Command: Make`
- `Laravel Artisan: Controller: Make`
- `Laravel Artisan: DB:Seed`
- `Laravel Artisan: Key: Generate`
- `Laravel Artisan: Migrate: Install`
- `Laravel Artisan: Migrate: Make`
- `Laravel Artisan: Migrate: Rollback`
- `Laravel Artisan: Migrate: Reset`
- `Laravel Artisan: Migrate: Refresh`
- `Laravel Artisan: Queue: Listen`
- `Laravel Artisan: Queue: Subscribe`
- `Laravel Artisan: Queue: Work`
- `Laravel Artisan: Session: Table`
- `Laravel Artisan: Custom Command`

##### Laravel Generate (Support for Jeffrey Way's [Laravel Generators](https://github.com/laracasts/Laravel-5-Generators-Extended):
- `Laravel Generate: Model`
- `Laravel Generate: Controller`
- `Laravel Generate: Seed`
- `Laravel Generate: View`
- `Laravel Generate: Migration`
- `Laravel Generate: Pivot Table`

##### Custom Commands
You can add custom commands.
Use `Preferences/Package Settings/Laravel 5 Artisan/Commands – User` menu item.

Simple command structure:

```json
[
    {
        "caption": "Laravel Artisan: Deploy Project",
        "command": "laravel5_artisan",
        "args": {
            "command": "deploy",
            "fill_in": true,
            "fill_in_lable": "Enter the branch name with options"
        }
    }
]
```

Change command `caption` and `command` in `args`.
Use `fill_in: true` if you need some input for your command and `fill_in_lable: "Text"` for message.

### Installation:
Use Package Controller or create a the directory `Laravel 5 Artisan` in your Sublime Text Packages directory with source code, and you're ready to go.

### Usage:
Press Cmd + Shift + P for the dropdown command list, search for `Laravel `, and pick your command. Also you can use `Tools/Laravel...` menu item

### Notes:
- Artisan file needs to been in the root folder of your structure in the sidebar.
- You need insert in Sublime Text user settings `"show_panel_on_build": true` or use `Tools/Build Results/Show Build Results` menu item for view results.
- Several commands do require [laracasts/generators](https://github.com/laracasts/Laravel-5-Generators-Extended) 
