# Handy Shortcuts and Command-Line Snippets for Developers

## Node / NPM
* `npm init -y` will run `npm init` and auto-confirm the default response prompt values.
* `npm i -S` is an alias for `npm install --save`: Updates `dependencies` in `package.json`
* `npm i -D` is an alias for `npm install --save-dev`: Updates `devDependencies` in `package.json`
* `npm i -O` is an alias for `npm install --save-optional`: Updates `optionalDependencies` in `package.json`
* `npm i -E` is an alias for `npm install --save-exact`: Updates `dependencies` in `package.json` with _exact version numbers_.

## Directory Navigation
* `cd ..` will navigate one directory back
* `cd ~` will navigate to your home directory
* `cd -` will change directory to your previous directory

## Pipe to Grep
Grep is a super powerful utility for searching text using string or regular expression patterns. To learn more on regular expressions, see our [handy guide](REGEX.md).
* `ps aux | grep [something]` will list all running processes matching the text or RegEx in `[something]`
* `[command] | grep [string/pattern]` will pipe the output of `command` to the `grep` utility to allow the result to be searched. See the section below on tailing a log file for another example of using `grep` with other commands.

## Working With Log Files
* `tail -f /var/log/apache2/error_log` - will stream a log file in real-time. Press `[CTRL]+C` to exit `tail`
* `cat /var/log/apache2/error_log` - will print the log file to the console
* `tail -f /var/log/apache2/error_log | grep 127.0.0.1` - will stream a log file, but will only print the lines containing the text '127.0.0.1'

## VIM / VI Commands
Ever get stuck in `vi`? Here are some basics. A much more comprehensive list can be found on [Lagmonster.org](http://www.lagmonster.org/docs/vi.html).
* `[ESC]:x` - Quit, saving changes
* `[ESC]:q` - Quit if there are no changes
* `[ESC]:wq` - Write file and Quit
* `[ESC]:q!` - Exit and ignore any changes
* `i` - Enable input at the cursor position
* `/string` - Search forward for string
* `?string` - Search backward for string
* `n` - Search for next instance of string
* `N` - Search for previous instance of string

## Custom Shortcuts in macOS / Unix / Linux
You can create `alias` commands in your `~/.bash_profile` file in macOS to create your own shortcut commands. For example, look at the following shortcut ideas:

```
alias ll='ls -lG'
alias add="git add"
alias commit="git commit -m"
alias s="git status"
alias rename="git branch -m"
alias b="git branch"
```