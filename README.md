# Half Knife Documentation

## [How to install the addon](./install.md)

## [Shortcut settings](./keymaps.md)

## Supported Blender versions
Tested on Blender 2.91. Newer versions will be supported as they comes up.

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

Make sure you have unchecked `On cage` button on every modifier, or cuts will go in wrong direction.

![](https://raw.githubusercontent.com/artempoletsky/half_knife_docs/master/img/4.png)

### Cut without preview option

To enable this option
1. Go to Blender preferences -> Addons
2. Find in list `Half knife`
3. Go to `Keymaps` tab
4. Open `Half knife` keymap, check `Cut without preview option`

![](https://raw.githubusercontent.com/artempoletsky/half_knife_docs/master/img/5.png)

Now you can do cuts without pressing mouse buttons.
When the operator is invoked from an outside of the mesh the preview will still be shown.

### Modal options
Similar to the default Blender knife features:

1. Shift: turn off snapping
2. Z: cut through

Slightly different with the default knife features:

1. Ctrl: snap to center. You can snap not only to the center of an edge or vertex but you can snap to the middle of a face too. Edges cutted in between the start and the end point will be cutted in a half. But preview of new vertices position will not be showed. When doing multi cuts this feature will act like "Alt: alternate snap to center."

2. Alt: alternate snap to center. You can still snap to center the start and the end, but edges in between will be cutted in a straight line.

3. С: angle constraint. Snapping to the half angle or the quarters between the active vertex (starting point) and linked edges. Active face, edges and verts will be highligted now. You need to mouse over linked to the starting point face to make it active. Unlikely in the default knife you can not snap to edge or vert in this mode. You can't activate this mode, when doing multicuts or when starting cut from the outside. With this you can create a right angle from the incoming point.

![](https://raw.githubusercontent.com/artempoletsky/half_knife_docs/master/img/angle_constraint.png)

4. H: Altitude mode. Another way to create the right angle at the end point. Creates an orthogonal edge from selected point, to edge you pointing. [See more.](./altitude.md)


## Not a 100% replacer of Blender default knife

With cutting concave ngons broken geometry can be occured.

By default Blender knife tool will be assingned on `Alt K` shortcut. You can change shortcuts in preferences.
