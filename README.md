## Welcome to Gonzo's fastfetch vault!

This repo was made as a spot to store my different configurations of fastfetch. It will be my exact config, so if anyone wants to use the set config, it is recomended to check the file to make sure all elements fit your style.  I.e. Custom gonzo ASCII


## Adding your own ASCII art

If you are wanting to use a config, and want to add in your own ASCII art(i.e. username, hostname, etc), I will explain the simplest method here. First download figlet or toilet to generate the ASCII art.  Once you have either or both of these, create whatever you want to use by running the following command in terminal.

``` bash
    figlet gonzo    <--- Your text here
    toilet gonzo    
    ```

This will give you your ASCII art, for this example i am using my name, but literally anything can be used.


``` bash
  __ _  ___  _ __  _______
 / _` |/ _ \| '_ \|_  / _ \
| (_| | (_) | | | |/ / (_) |
 \__, |\___/|_| |_/___\___/
 |___/ 
```
Once you have your ascii, find the space you wish to insert it in fastfetch.  Follow this format

``` jsonc
...Beginning of your fastfetch..
{
    "type": "custom",
    "format": "  __ _  ___  _ __  _______ "
},
{
    "type": "custom",
    "format":" /  ` |/   \\| '  \\|   /   \\"
},
## And so on ###
...rest of the fastfetch
```

Note: If your ASCII includes backspaces, notice how we have to define them twice.  This is to avoid errors.  If you recieve an error on attempting to run the config, check your ASCII!!

