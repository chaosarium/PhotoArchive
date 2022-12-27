## Demo

Demo: https://gallerybeta-chaosarium.wunderbucket.dev/

## How to use

Install [thumbsup](https://thumbsup.github.io/) and its dependencies

Create a `config.json` file somewhere with the following information:

```json
{
    "input": ".../input", // path to photo input folder
    "output": ".../output", // where to generate output

    // See https://thumbsup.github.io/docs/3-configuration/cheat-sheet/ 
    // for what these do
    "small-size": "300", 
    "large-size": "1200",
    "cleanup": "false",
    "album-page-size": "0",
    "albums-output-folder": "albums",

    // If you want to watermark your photos
    "watermark": ".../watermark.png", // path to watermark png
    "watermark-position": "SouthEast", // location

    "theme-path": ".../archive", // path to the root of this repo

    "title": "PhotoArchive", // Website title
    "footer": "these are placeholder images from unsplash", // website footer

    "dummy": "dummy" // this does nothing (*ﾟ▽ﾟ*)
}
```

Then run the following to generate static website

```bash
thumbsup --config "path/to/config.json"
```