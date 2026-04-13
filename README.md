# StreamLife 🎙️

A modern, multi-stream audio player with a premium dark interface inspired by Europe 1. Listen to multiple radio streams simultaneously with an intuitive, glass-morphic design.

## Features

- 🎵 **Multi-Stream Support** - Add and manage multiple audio streams
- 🎨 **Premium Dark Theme** - Glassmorphic design with vibrant blue accents
- 🎛️ **Advanced Controls** - Play, pause, skip, shuffle, repeat, volume control
- 🔄 **Stream Management** - Add, remove, and switch between streams seamlessly
- 📱 **Responsive Design** - Works on desktop, tablet, and mobile
- 🎯 **Real-time Status** - See active streams and playback information

## Quick Start

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No dependencies required - vanilla HTML/CSS/JavaScript

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/streamlife.git
cd streamlife
```

2. Open the application:
```bash
# Simply open index.html in your browser
open index.html
```

Or use a local server:
```bash
python -m http.server 8000
# Then visit http://localhost:8000
```

## Usage

### Adding a Stream

1. Click the **"Add Stream"** button in the header or sidebar
2. Fill in:
   - **Stream Name** - e.g., "France Musique"
   - **Stream URL** - The streaming URL (HLS, RTSP, etc.)
   - **Genre** (optional) - e.g., "Classical", "Jazz"
3. Click **"Add Stream"** to save

### Playing a Stream

1. Select a stream from the **"Your Streams"** list
2. Click the **play button** or the **play icon** on the stream card
3. Use the floating player bar at the bottom to control playback

### Managing Streams

- **Delete Stream** - Hover over a stream card and click the delete icon
- **Switch Streams** - Click on a different stream to make it active
- **Volume Control** - Use the volume slider in the player bar

## Project Structure

```
streamlife/
├── index.html          # Main application file
├── README.md           # This file
├── DESIGN.md           # Design system documentation
├── package.json        # Project metadata (for future npm setup)
└── assets/             # (Future) Icons and images
```

## Design System

StreamLife uses "The Ethereal Broadcaster" design system - a high-end editorial framework with:

- **Colors**: Deep charcoal backgrounds with vibrant blue accents (#b2c5ff)
- **Typography**: Manrope for headlines, Inter for body text
- **Depth**: Glassmorphic panels with backdrop blur effects
- **Spacing**: Consistent rhythm using tailwind spacing scale

See `DESIGN.md` for complete design guidelines.

## Browser Support

- Chrome/Chromium 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## Stream URL Formats Supported

- HLS (.m3u8)
- RTSP
- HTTP Progressive Download
- Other browser-compatible formats

**Note**: Cross-origin streaming may require CORS headers on the source server.

## Known Limitations

- Audio playback requires valid stream URLs with proper CORS headers
- Some protected streams may not work due to security restrictions
- Mobile browsers may have different audio permissions

## Future Enhancements

- [ ] Local storage for saved streams
- [ ] Stream metadata display (currently playing song)
- [ ] Equalizer controls
- [ ] Recording capability
- [ ] Stream quality selection
- [ ] Dark/Light theme toggle
- [ ] Export/import stream lists
- [ ] Mobile app (React Native/Flutter)

## Contributing

Contributions are welcome! Please feel free to:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Credits

- Design inspiration: Europe 1 Radio UI
- Icons: Google Material Symbols
- Fonts: Manrope & Inter from Google Fonts
- CSS Framework: Tailwind CSS

## Support

For issues, feature requests, or questions:
- Open an [Issue](https://github.com/yourusername/streamlife/issues)
- Check existing issues for solutions
- Include browser info and stream URLs when reporting bugs

---

**Made with ♥ for radio enthusiasts and audio lovers everywhere.**
