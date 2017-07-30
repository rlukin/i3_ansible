# What is this?
Playbook for ansible that install i3wm with other essentials for desktop enviroment and some usefull tools.
Usefull for new workstation fast setup.

# Basic enviroment installation and tuning
ansible-playbook -i '192.168.1.36,' steps.yml -u roman -kK
## Requirements:
 - ansible >= 2.1
 - openssh-server on target

# Firefox ricing
 - Plugins
  * vimfx
  * stylish
  * hide caption titlebar plus 
  * firebug 
  * Arc Darker Theme, Arc Dark Theme

## For firefox use stylish. Create a theme whith that supa dark theme fix:
by default firefox dont change background for input fields, so you have grey text on white background
```
input:not(.urlbar-input):not(.textbox-input):not(.form-control):not([type='checkbox']) {
    -moz-appearance: none !important;
    background-color: white;
    color: black;
}

#downloads-indicator-counter {
    color: white;
}

textarea {
    -moz-appearance: none !important;
    background-color: white;
    color: black;
}

select {
    -moz-appearance: none !important;
    background-color: white;
    color: black;
}
```
