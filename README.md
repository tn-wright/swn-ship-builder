# SWN Ship Builder
A simple utility to assist in creating ships for the revised edition of Stars Without Number, a game by Kevin Crawford. The tool is built using Vue 2.

## Usage
To start, select a hull type from the drop down menu. The initial stats of that hull will be displayed after one is selected. In addition, fields to add fittings, defenses, and weapons will also appear after the hull type is picked.

To add a fitting, simple select it from the drop down menu in the appropriate category. The fitting listings provide the base stats of the fitting to aid in selection. The minus button next to each item can be used to remove the fitting, and the text field can be used to change the quantity. The "Add X" button along the top of each section can be used to add additional selectors for more fittings within that category.

As fittings are selected, the current ship stats will be displayed along the bottom. This included the remaining power, mass, and hard points the hull has. The tool does not prevent invalid configurations, but will color the final stats red if something is incorrect, like using more mass than the hull has available. 

The tool does not currently support the mods provided by the core rulebook, only the fittings and hulls. 

## Adding More Options
The options are all provided using JSON, found within the `<script>` of `shipbuilder.html`. To add additional options, simple add another item to the appropriate array. It is important to use the same template as the existing options, as it is assumed the fields of the template exist. 
