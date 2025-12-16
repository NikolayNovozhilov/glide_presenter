# Glide Presenter

A lightweight, browser-based presentation tool that transforms SVG files into dynamic, zoom-and-glide presentations. Simple and built for technical diagrams.

![Glide Presenter Demo](demo.gif)

Try it [LIVE!](https://nikolaynovozhilov.github.io/glide_presenter/)

## What Does This App Do?

Glide Presenter lets you create engaging, non-linear presentations from any SVG file. Instead of traditional slide-by-slide presentations, you can:

- **Zoom and pan** smoothly through your visual content
- **Define keyframes** to guide your presentation flow
- **Selectively hide/show elements** to control what your audience sees at each moment
- **Export as a single HTML file** containing everything - no server required and cross-platform

Perfect for technical diagrams, infographics, mind maps, architecture diagrams, or any visual content created in tools like Excalidraw, Figma, Illustrator, or any SVG editor.

## Why Build Yet Another Presentation Tool?

This project was inspired by **Bobby Broccoli's Videos** ([YouTube Channel](https://www.youtube.com/user/BobbyBroccoli)) However, they're created in Blender - powerful but too complex. I wanted something very simple.

There is this **Excalidraw-Obsidian Slideshow plugin** ([Demo](https://www.youtube.com/watch?v=JwgtCrIVeEU))
However the setup and usage are quite complex. Especially since I'm not an Obsidian user. The learning curve felt too steep for my specific task.

**Sozi** is the closest match. However, I found it difficult to selectively hide content - a crucial feature for controlling narrative flow and what the audience sees at each moment. This was a dealbreaker for me. Additionally, the project's complexity made it challenging to modify or extend. I borrowed some concepts from it though.

**The Solution:** I made my own app - Glide Presenter - that focuses on simplicity and one key feature that others lack - **easy content visibility control**. You can click to hide any SVG element in any frame, making it trivial to build up complex diagrams progressively or create reveal effects.

## Vibe-Coded: An AI-Assisted Development Experiment

This project is an experiment in AI-assisted development. Full transparency: I didn't write a single line of code myself. I can code python all right, but didn’t touch JavaScript for years.

It took ~25 prompts given to Claude Sonnet 4.5 (browser chat, not Claude Code). I briefly tried Google AI Studio (Gemini Pro Preview) and I kept quite a bit of UI/CSS suggested by it. But ultimately I switched back to Claude because of speed.

*I may write a more detailed post about the workflow, lessons learned, and effective prompting strategies later.*

## 🚀 Quick Start

### Option 1: Use Online (Recommended)
Visit the [live demo](https://nikolaynovozhilov.github.io/glide_presenter/) and click "Launch Glide Presenter App"

### Option 2: Download and Run Locally
1. Download `presenter_app.html`
2. Open it in any modern web browser (Chrome, Firefox, Safari, Edge)
3. That's it! No installation or server required.

## 📖 How to Use

### Creating Your First Presentation

1. **Load Your SVG**
   - Click "Load SVG File" and select your SVG diagram
   - The SVG is never edited by the app. All frame data is stored in JSON file separately. 
   - You can keep editing your SVG diagram. The app generates stable hash-based IDs for SVG elements. You can move/resize elements without breaking hidden element references.
   - I use [Excalidraw](https://excalidraw.com/) to create diagrams and then export to SVG.  

2. **Create Frames**
   - Use **zoom buttons (+/−)** or **mouse wheel** to zoom in/out
   - **Click and drag** to pan around your content
   - Click **"Add Frame"** to save the current view as a keyframe
   - Repeat to create multiple frames showing different parts or zoom levels

3. **Hide Elements** (Optional)
   - Click **"Toggle Hide Mode"** to enable element selection
   - Click any SVG element to hide it in the current frame
   - Hidden elements appear in the sidebar - click "Show" to unhide them
   - Perfect for progressive disclosure or reveal effects

4. **Test Your Presentation**
   - Click **"Play Presentation"** to enter presentation mode
   - Use **arrow keys**, **space**, or **Page Up/Down** to navigate
   - Press **Escape** to exit presentation mode

5. **Save JSON**
   - You can save your work as a JSON file and come back to editing later

6. **Export**
   - Click **"Publish Standalone HTML"** to export
   - Share the single HTML file - it contains everything embedded
   - Recipients just open it in a browser - no app needed!

### Keyboard Shortcuts (Presentation Mode)

| Key | Action |
|-----|--------|
| `→` `Space` `Page Down` | Next frame |
| `←` `Page Up` | Previous frame |
| `Esc` | Exit presentation mode |


## Contributing

Contributions are welcome! Whether it's:
- Bug reports
- Feature suggestions
- Code improvements
- Sample presentations
- Documentation improvements

Feel free to open an issue or submit a pull request.

### Have You Created Something Cool?

If you've made a presentation with Glide Presenter that you'd like to share, please submit a pull request or send it my way! I'll be happy to feature it in the samples section.

## 📄 License

MIT License - feel free to use, modify, and distribute as you wish.

## 🙏 Acknowledgments

- Inspired by [Bobby Broccoli's](https://www.youtube.com/user/BobbyBroccoli) educational videos
- Concepts borrowed from [Sozi](https://sozi.baierouge.fr/)
- Built entirely with Claude Sonnet 4.5 by Anthropic

## 📬 Contact

For questions, suggestions, or just to share what you've built:
- Open an issue on GitHub
