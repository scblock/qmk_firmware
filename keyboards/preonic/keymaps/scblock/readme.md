# Steve's Keyboard Layout

Effectively the default Preonic layout, with minor quality of life optimizations, and revised for the 2020 Drop of rev3 boards with pre-soldered RGB LEDs and no backlighting to control LED color, pattern, brightness, etc.

## Key Changes

This layout makes several quality of life changes for me, including:

- Escape key at Caps Lock position is also Control when held. The macro ``#define CTL_ESC LCTL_T(KC_ESC)`` is employed to simplify writing this.
- The default Enter key at the Right Shift location pulls double duty as right shift when held using ``KC_SFTENT``.
- A new layer is added to manage both LED lighting controls (pre-soldered to the board in this Drop) to the left side of the board and add a 10-key data entry pad to the right side.
- The keyboard does not have backlighting, and so the BRITE key as defined in the default Preonic layout does not seem to be of use. This layout revises the bottom left key to turn on or toggle on the new LED control and 10-key data entry layer.

This is still very much a work in progress as I get used to the small form factor board. I'm considering revising arrow keys to use Vim bindings, but have not done that yet as I would need to find new locations for the -=[]_+{} symbols. I'm reviewing other keymaps and considering ideas, but will take it slow. Caps Lock may return, as I occasionally find use for it.


## Layers

1. QWERTY - Default keymap, with my modifications
2. COLEMAK - Colemak layout, with my modifications
3. DVORAK - Dvorak layout, with my modifications
4. LOWER - Lower key, same as default KB layout
5. RAISE - Raise key, same as default KB layout
6. LEDTK - New LED underlighting adjustment and 10-key layout. Hold the LED/10Key key on base layout to activate momentarily, double tap to toggle layer on and off for numeric data entry.
6. ADJUST - Lower+Raise, same as default KB layout

### QWERTY
```
,-------------------------------------------------------------------------------------------.
|     `    |   1  |   2  |   3  |   4  |   5  |   6  |   7  |   8  |   9  |   0  | Bksp     |
|----------+------+------+------+------+------+------+------+------+------+------+----------|
| Tab      |   Q  |   W  |   E  |   R  |   T  |   Y  |   U  |   I  |   O  |   P  | Del      |
|----------+------+------+------+------+-------------+------+------+------+------+----------|
| Ctrl/Esc |   A  |   S  |   D  |   F  |   G  |   H  |   J  |   K  |   L  |   ;  |    "     |
|----------+------+------+------+------+------|------+------+------+------+------+----------|
| Shift    |   Z  |   X  |   C  |   V  |   B  |   N  |   M  |   ,  |   .  |   /  |RShft/Ent |
|----------+------+------+------+------+------+------+------+------+------+------+----------|
| LED/10Key| Ctrl | Alt  | GUI  |Lower |    Space    |Raise | Left | Down |  Up  |Right     |
`-------------------------------------------------------------------------------------------'
```

### Colemak
```
,-------------------------------------------------------------------------------------------.
|     `    |   1  |   2  |   3  |   4  |   5  |   6  |   7  |   8  |   9  |   0  | Bksp     |
|----------+------+------+------+------+------+------+------+------+------+------+----------|
| Tab      |   Q  |   W  |   F  |   P  |   G  |   J  |   L  |   U  |   Y  |   ;  | Del      |
|----------+------+------+------+------+-------------+------+------+------+------+----------|
| Ctrl/Esc |   A  |   R  |   S  |   T  |   D  |   H  |   N  |   E  |   I  |   O  |    "     |
|----------+------+------+------+------+------|------+------+------+------+------+----------|
| Shift    |   Z  |   X  |   C  |   V  |   B  |   K  |   M  |   ,  |   .  |   /  |RShft/Ent |
|----------+------+------+------+------+------+------+------+------+------+------+----------|
| LED/10Key| Ctrl | Alt  | GUI  |Lower |    Space    |Raise | Left | Down |  Up  |Right     |
`-------------------------------------------------------------------------------------------'
 ```
 
 ### Dvorak
 ```
 ,-------------------------------------------------------------------------------------------.
 |     `    |   1  |   2  |   3  |   4  |   5  |   6  |   7  |   8  |   9  |   0  | Bksp     |
 |----------+------+------+------+------+------+------+------+------+------+------+----------|
 | Tab      |   "  |   ,  |   .  |   P  |   Y  |   F  |   G  |   C  |   R  |   L  | Del      |
 |----------+------+------+------+------+-------------+------+------+------+------+----------|
 | Ctrl/Esc |   A  |   O  |   E  |   U  |   I  |   D  |   H  |   T  |   N  |   S  |    /     |
 |----------+------+------+------+------+------|------+------+------+------+------+----------|
 | Shift    |   ;  |   Q  |   J  |   K  |   X  |   B  |   M  |   W  |   V  |   Z  |RShft/Ent |
 |----------+------+------+------+------+------+------+------+------+------+------+----------|
 | LED/10Key| Ctrl | Alt  | GUI  |Lower |    Space    |Raise | Left | Down |  Up  |Right     |
 `-------------------------------------------------------------------------------------------'
 ```
 
 ### Lower
 ```
,-----------------------------------------------------------------------------------.
|   ~  |   !  |   @  |   #  |   $  |   %  |   ^  |   &  |   *  |   (  |   )  | Bksp |
|------+------+------+------+------+-------------+------+------+------+------+------|
|   ~  |   !  |   @  |   #  |   $  |   %  |   ^  |   &  |   *  |   (  |   )  | Del  |
|------+------+------+------+------+-------------+------+------+------+------+------|
| Del  |  F1  |  F2  |  F3  |  F4  |  F5  |  F6  |   _  |   +  |   {  |   }  |  |   |
|------+------+------+------+------+------|------+------+------+------+------+------|
|      |  F7  |  F8  |  F9  |  F10 |  F11 |  F12 |ISO ~ |ISO | |      |      |      |
|------+------+------+------+------+------+------+------+------+------+------+------|
|      |      |      |      |      |             |      | Next | Vol- | Vol+ | Play |
`-----------------------------------------------------------------------------------'
 ```
 
 ### Raise
 ```
,-----------------------------------------------------------------------------------.
|   `  |   1  |   2  |   3  |   4  |   5  |   6  |   7  |   8  |   9  |   0  | Bksp |
|------+------+------+------+------+------+------+------+------+------+------+------|
|   `  |   1  |   2  |   3  |   4  |   5  |   6  |   7  |   8  |   9  |   0  | Del  |
|------+------+------+------+------+-------------+------+------+------+------+------|
| Del  |  F1  |  F2  |  F3  |  F4  |  F5  |  F6  |   -  |   =  |   [  |   ]  |  \   |
|------+------+------+------+------+------|------+------+------+------+------+------|
|      |  F7  |  F8  |  F9  |  F10 |  F11 |  F12 |ISO # |ISO / |      |      |      |
|------+------+------+------+------+------+------+------+------+------+------+------|
|      |      |      |      |      |             |      | Next | Vol- | Vol+ | Play |
`-----------------------------------------------------------------------------------'
```

### LED/10-Key
```
,-------------------------------------------------------------------------------------.
|   LED  |      |      |      |      |      |      |      | Num  |      |      |      |
| Toggle |      |      |      |      |      |      |      | Lock |   /  |   *  |   -  |
|--------+------+------+------+------+------+------+------+------+------+------+------|
|        |Mode+ |Brite+|Hue + |Sat + |      |      |      |   7  |   8  |   9  |   +  |
|--------+------+------+------+------+-------------+------+------+------+------+------|
|        |Mode- |Brite-|Hue - |Sat - |      |      |      |   4  |   5  |   6  |   +  |
|--------+------+------+------+------+------|------+------+------+------+------+------|
|        |Mode P|Mode B|Mode R|ModeSW|      |      |      |   1  |   2  |   3  | Enter|
|--------+------+------+------+------+------+------+------+------+------+------+------|
|        |ModeSN|Mode K|Mode X|Mode G|             |      |   0  |   0  |   .  | Enter|
`-------------------------------------------------------------------------------------'
 ```
