# Half Knife Documentation

[How to install the addon](./install.md)

## Supported Blender versions
Tested on Blender 2.82a and 2.83 beta. Newer versions will be supported as they comes up. 

## Usage

### Without initial selection
1. Mouse over on the mesh where you want to start the cut. 
2. Press `K`, mouse over the place on the mesh where you want to be end of the cut. 
3. Press `left mouse button`

### With selection 
1. Press `K`, mouse over the place on the mesh where you want to be end of the cut. 
2. Press `left mouse button`

A maximum of 10 initial vertices can be selected. The limitation is made for performance reasons and to exclude accidental use.
You can do multicuts from face or edge mode. Selected edge in this case counts as 2 vertices. Selected face counts as (N) vertices selecected.

## Working with modifiers  

Make shure you have unchecked `On cage` button on every modifier, or cuts will go in wrong direction.

![](https://raw.githubusercontent.com/artempoletsky/half_knife_docs/master/img/4.png)

### Cut without preview option

To enable this option
1. Go to Blender preferences -> Addons
2. Find in list `Half knife`
3. Go to `Keymaps` tab
4. Open `Half knife` keymap, check `Cut without preview option`

![](https://raw.githubusercontent.com/artempoletsky/half_knife_docs/master/img/5.png)

Now you can do cuts without pressing mouse buttons. 

## Not a replacer of Blender default knife

1. You can't do cuts from outside of the mesh
2. With cutting concave ngons broken geometry can be occured. 

By default Blender knife tool will be assingned on `Alt K` shortcut. You can change shortcuts in settings. 


