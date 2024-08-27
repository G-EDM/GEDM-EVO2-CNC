To print the big parts wihout warping it is necessary to add some adhesive to the printbed and change the support settings to get a stronger bond between model and supports. Another thing that is highly recommended is to add some kind of dust wiper to the filament. 

The print may take long and a few dust particle can lead to a clogged nozzle. A simple DIY dust wiper can be made with a zip tie and a piece of old lint free cloth. I have two dust wipers on the filament. Both are hook and loop fasteners wrapped around the filament with the fluffy part on the inside. Neoprene works too. A dust wiper can be the main problem solver on very long prints.

As adhesive I use a thick layer of strong hairspray on an ender 3v2 bed. Works very well but may not work at all on some specific printbeds used on other printers. Don't know what adhesive should be used on flexible beds.

It is also needed to add a brim. The default brim I use is 20mm. This is not possible for all parts. It is possible to use a smaller brim and then use cura patches on critical edges.

Another thing are the supports. After reinstalling my OS with a fresh cura install the supports stopped touching the print and even small chamfers on smaller parts started warping. This can be fixed in the cura settings.


Support Z Distance
Support X/Y Distance

Reducing this values will bring the support closer to the model.

Usinf 0.2mm for both of those settings will provide a strong fuse between support and model. This is good for the big parts. Note that the supports are hard to remove and this settings will only work for the big parts to prevent warping.

The big parts are printed with supports touching build plate. So it is Ok to have the supports fused to the model.

Also enable support interface. This will generate a support roof that help with fusing.

Support Distance Priority set to Z overrides X/Y. This is also necessary. With the Z axis moving up the XY distancae of the support will get smaller-



Thanks to 3dprinterly for his nice explaination:
https://3dprinterly.com/how-to-fix-cura-supports-not-touching-model-or-print/


Best way is to create a custom print profile for the heavy prints and use another for the normal prints where we want to easily remove the supports and don't have big risk of warping.
