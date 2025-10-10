# SpriteFrames exported textures

An addon that exposes the texture resources that are internally used by SpriteFrames resources, allowing replacing them by other textures.

The main use case for this addon is editing a SpriteFrames by swapping the spritesheets it uses.

![Spriteframes selected in godot editor. It shows the bottom dock where the animations of the spriteframes resource can be edited. Also, it shows the inspector, where a new property appears for each texture the SpriteFrames has.](media/spriteframes_as_seen_from_inspector.png)

--------------

Replacing a texture by another updates all animations that were using frames created from that texture:

![The gif image shows a spriteframes resource opened in Godot. It displays several properties in the inspector, one for each texture that is used by the spriteframe. Then, new images are dragged and dropped where one of the original textures were, and the current animation from the spriteframe automatically changes its frames to reflect this change.](media/replace_texture_in_spriteframes.gif)

Only allows replacing textures by other textures of the same exact size:

![The gif image shows a spriteframes resource opened in godot. A texture is dragged and dropped to the inspector, trying to replace one of the spriteframes' textures. Nothing changes in the spriteframes and a notification appears in the editor, saying "New texture size is (1152x192) doesn't match old texture size (768x192)"](media/reject_incorrect_texture_replacement_in_spriteframes.gif)
