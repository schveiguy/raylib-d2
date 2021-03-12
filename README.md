# NOTE
This is a resurrected copy of onroundit's raylib-d package. I've released 3.1.0 which is identical to 3.0.3 with a fix for a bug in the header (I don't have the original bug report because the original github repo is gone) but with the name changed to avoid naming conflict on code.dlang.org. I also fixed the name in all the original tags, so all you should need to do is update your raylib-d dependency to raylib-d2.

![](raylib_logo.png)

# raylib-d2 [![DUB](https://img.shields.io/dub/v/raylib-d2?style=for-the-badge)](https://code.dlang.org/packages/raylib-d2)
(static) D bindings for [raylib](https://www.raylib.com/), a simple and easy-to-use library to learn videogames programming.

# Installation
`dub add raylib-d`

## First, get a copy of Raylib
You can get the library by compiling it from the [source](https://github.com/raysan5/raylib), download the [official precompiled binaries](https://github.com/raysan5/raylib/releases) or [download them from our repository](https://github.com/onroundit/raylib-d/releases) (originally taken from official releases, sorted in folders for each system).

## In order to link against raylib, add it to your dub.json.
```json
"libs": [ "raylib" ]
```
For more information look into the [wiki](https://github.com/onroundit/raylib-d/wiki/Installation).

# Example
```D
import raylib;

void main()
{
	InitWindow(800, 600, "Hello, Raylib-D!");
	while (!WindowShouldClose())
	{
		BeginDrawing();
		ClearBackground(Colors.RAYWHITE);
		DrawText("Hello, World!", 400, 300, 28, Colors.BLACK);
		EndDrawing();
	}
	CloseWindow();
}
```

# [Docs / cheatsheet](https://github.com/onroundit/raylib-d/wiki/Docs-(cheatsheet))

# License
raylib-d is licensed under an unmodified zlib/libpng license. View [LICENSE](LICENSE).
