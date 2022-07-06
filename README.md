# dmenu-conky-todo
A super light todo list using conky and dmenu.

This repo contains 3 files:

todo which is a bash file and runs a simple todo list app with dmenu,

todo.conkyrc which is the conky config,

And color_scheme that is another script for adding some sense to this simple todo list.

There is no executable application to start this todo list, there is 2 scripts here and you should map a short-key to run them.

# TODO Script
todo script will open a dmenu that will show you all todos and you can either remove them or add a new one.

![screenshot_20220706-203752_1920x1080](https://user-images.githubusercontent.com/33146532/177643716-01dc5b52-8fcd-439a-85b6-78eb5bcb9eca.png)

# color_scheme Script
First you should move todo.conkyrc file to '~/.config/wal/' directory.

You should also create '~/.dmenu-conky-todo/todo_qoutes' file containig some (inspiring) qoutes to be randomly selected and be placed at the top of todo conky.

This script will pick a random picture from '~/Pictures/wallpaper/' directory and set it as your background, and also extract some colors based on colors in the chosen picture.

Then will regenerate a new todo.conkyrc file which contains the random qoute and uses the extracted colors.

# todo.conkyrc File
This file is the base file which is going to be used for creating the conkyrc file.

After running the color_scheme script, the new conkyrc file will be in '~/.cache/wal/todo.conkyrc'.

add this command to startup script of your system to have it allways running:

``` bash
conky -c ~/.cache/wal/todo.conkyrc
```

Thats it, you will have this result updating every second. you can modify your todo list by running todo script.

![screenshot_20220706-194753_1920x1080](https://user-images.githubusercontent.com/33146532/177646129-a76f1242-933a-49a0-9933-e70ea57f4f74.png)
![screenshot_20220706-194805_1920x1080](https://user-images.githubusercontent.com/33146532/177646141-4c95b79f-733d-43ad-9897-2844718e23cd.png)
![screenshot_20220706-194924_1920x1080](https://user-images.githubusercontent.com/33146532/177646155-aefd0d5a-5fe3-4e2d-88ba-b81507bcee06.png)
![screenshot_20220706-194839_1920x1080](https://user-images.githubusercontent.com/33146532/177646145-2b9f0fe5-5c95-4a66-b0f9-c171606028b4.png)
![screenshot_20220706-200042_1920x1080](https://user-images.githubusercontent.com/33146532/177646162-f11ced92-0c8f-4df6-a889-978808c8bd32.png)

And This is my desktop with this dmenu-conky-todo:
![screenshot_20220707-015837_1920x1080](https://user-images.githubusercontent.com/33146532/177646737-605003da-a635-4b59-a477-765ffce2b095.png)
