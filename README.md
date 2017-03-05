#ArkTrace
###A debugging tool for mod authors working on projects for ARK: Survival Evolved

#####Instructions:
1. Copy the arktrace folder into your mods project folder.
2. Add the ArkTrace_Manager_BP to your PGD as a singleton actor.
3. Open the ArkTrace_Manager_BP.
..* Go to the event graph and find the "Switch on string" that follows the delegate event.
..* Change the [Mod Name] part of the string.
4. In any part of your mod you should be able to add a macro "Create Live Event Trace Log".
..* Add a string for entry, a priority, and (if applicable) any related object *other than the object logging the event*.
5. In game, open the console and enter the command 'AdminCheat ScriptCommand ArkTrace <modname>'