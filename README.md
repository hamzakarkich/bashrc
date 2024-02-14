# PS1
Customizing the Shell Prompt (PS1) transforms the command-line interface. Users edit the PS1 variable in their shell config, adjusting elements like username, hostname, and directory, often adding colors. This enhances both functionality and aesthetics for efficient and personalized shell interactions.

![PS1](https://github.com/hamzakarkich/bashrc/blob/main/img/Screenshot%202024-02-14%20145057.jpg)

To change the PS1 prompt in Bash, you need to modify the PS1 variable in your shell configuration file. Typically, this file is either `~/.bashrc` or `~/.bash_profile`. Here's a step-by-step guide:

1. Open your preferred text editor. For example, you can use the "nano" editor:

```bash
nano ~/.bashrc
```

2. Look for the line that sets the PS1 variable. It usually starts with `PS1=`.

3. Customize the PS1 variable according to your preferences. You can include various escape sequences for information like username (`\u`), hostname (`\h`), current working directory (`\w`), and more. You can also add color codes for better visual appeal.

4. Save the changes and exit the text editor.

5. To apply the changes immediately, you can either restart your terminal or run:

```bash
source ~/.bashrc
```

To customize your shell prompt with colors and variables, modify the PS1 variable in your shell configuration file. Here's an example for Bash:

1. Open your shell configuration file:

   ```bash
   nano ~/.bashrc
   ```

2. Locate the PS1 variable, which defines your prompt.

3. Customize the PS1 variable by adding color codes and variables. Here's an example:

   ```bash
   PS1='\[\e[1;32m\]\u@\h\[\e[0m\]:\[\e[1;34m\]\w\[\e[0m\]\$ '
   ```

   - `\u`: Username
   - `\h`: Hostname
   - `\w`: Current working directory
   - `\e[1;32m`: Bold green color code
   - `\e[1;34m`: Bold blue color code
   - `\e[0m`: Reset color attributes

   You can customize the order and appearance of these elements.

4. Save the changes and exit the editor.

5. Apply the changes to your current session:

   ```bash
   source ~/.bashrc
   ```

Now, your shell prompt will display the username in bold green, followed by the hostname, a colon, the current working directory in bold blue, and the `$` symbol.
