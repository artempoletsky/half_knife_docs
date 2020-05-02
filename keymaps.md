# Keymaps settings

The author thinks that it is more convenient for new users to use the preview by default.
For expirienced users perhaps more useful to switch the `K` and the `shift K` shortcuts.

## Adding a new shortcut

After pressing the `Add new` button, you will see a new keymap item. 

![](https://raw.githubusercontent.com/artempoletsky/half_knife_docs/master/img/keymaps2.png)

All operator settings will be inactive and highlighted with gray color.
Because the `mesh.half_knife_operator` can be used as both modal and not modal operator, you need to specify all settings of the operator.
They all must be active like in the image below. Otherwise your shortcut will "remember" the setting from the last use.

![](https://raw.githubusercontent.com/artempoletsky/half_knife_docs/master/img/keymaps3.png)

Here is an example of a new custom shorcut. It can be used as quick edge subdivide.  
With nothing is selected, mouse over an edge, and press `ctrl K`.

### Troubleshoting

If you create a keymap item that exactly the same as any other keymap item, it will disapear. This is a default blenders behavior.
This will happen when you press `Add new` and make all operator settings active and unchecked, for example. 
