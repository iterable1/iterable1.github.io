# NASA Mission Hardware Trail

An interactive, globe-based guide to the hardware NASA has left across Earth, the Moon, Mars, and deep space. It is designed to help school-age space enthusiasts connect spacecraft and instruments with the science they enabled.

## Project objective

Since the 1960s, NASA missions have left landers, rovers, experiment packages, and other hardware on worlds across the solar system. Some completed their planned science; some operated far beyond their expected lifetimes; others are still traveling through deep space. This project turns that history into an approachable, visual story about what the hardware did, what scientists learned, and what remains.

## Explore

- **Earth:** Visit launch, training, re-entry, and spacecraft-disposal locations that provide context for missions beyond Earth.
- **Moon:** Explore Apollo landing sites and the equipment and experiments left on the lunar surface.
- **Mars:** Visit landers and rover sites, along with a polar science stop that introduces Mars' seasonal ice.
- **Deep Space:** Browse a spacecraft carousel featuring Voyager 1, Voyager 2, and New Horizons.

Select a pin or spacecraft to open its mission guide. Guides include mission status, objectives, instruments and hardware, science results, longer-form explanations, trivia, relevant imagery, image credits, and links to further information. Globe controls support rotation and zoom, and a scale helps put distances in context. Text-to-speech controls let visitors listen to the guide sections in supported browsers.

## Run locally

The project is a static website and does not require a build step or backend. Keep the HTML file and the two local map textures in the same folder.

1. Open a terminal in this project folder.
2. Start a local web server:

   ```powershell
   py -m http.server 8000
   ```

   If `py` is not available, use `python -m http.server 8000` or a local static-server extension in VS Code.
3. Open <http://localhost:8000/interactive_3d_earth_nasa_residues.html> in a modern browser.

The page uses WebGL and loads Three.js and many mission images from external sources, so an internet connection is needed for all content to appear. Text-to-speech uses the browser's built-in Speech Synthesis API and requires browser support and an available system voice.

## Project files

- `interactive_3d_earth_nasa_residues.html` - application, mission content, styles, and interactive behavior.
- `moon_lroc_color_2k.jpg` - local lunar map texture.
- `mars_color_2k.jpg` - local Mars map texture.
- `LICENSE` - project license.

## Sources and educational use

Mission-specific references and image credits are linked from the relevant guides. The project primarily directs visitors to NASA mission pages and the NASA Image and Video Library, with additional sources where appropriate. Mission status and science summaries are educational snapshots, not a live spacecraft-status feed; follow the linked sources for current information and deeper research.

## License

This project is distributed under the MIT License. See [LICENSE](./LICENSE).

