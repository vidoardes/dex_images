## Dex Images

### Keep track of your little monsters

A repository containing the main Pokemon icons from PokemonGo with the transparent

Built using ImageMagick

### Project Setup

#### Requirements

* ImageMagick 7.0

**Massive thank you to Chrales**, whos work on updating the assets from PoGO makes this app looks so good! [You can find his repo here.](https://github.com/ZeChrales/PogoAssets)

To normalise the images and trim the empty space, you can install [ImageMagick](https://imagemagick.org/script/download.php) and run the following command:

Windows Powershell:

```Powershell
Foreach ($f in Get-ChildItem *.png) {
    magick "$f" -fuzz 15% -trim +repage "$f"
}
```

Unix / Linux Bash:

```bash
for f in ./*.png; do
magick "$f" -fuzz 15% -trim +repage "$f";
done
```

Play around with the parameters to see what you can do, ImageMagick is a very powerful tool.