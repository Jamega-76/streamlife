# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-04-13

### Added
- 🎙️ **Multi-Stream Support**: Add and manage multiple audio streams simultaneously
- 🎵 **30 Pre-loaded Europe 2 Streams**: Europe 2 New, Classics, Acoustic, Hits, Rock, Mix, Live, Nouvelle Scène, 100% Français, Slow, Cardio, 90's, Millenium, Girl Power, Pop Rock, French Touch, Love, Pop 2010, Dance, Ciné, Pop 2020, Running, Duos, Soul/R'n'B, Home, Work, Zen, and 3 additional streams
- 🎨 **Premium Dark Theme**: Glassmorphic design with vibrant blue accents (#b2c5ff)
- 🎛️ **Full Playback Controls**: Play, pause, skip previous, skip next, shuffle, repeat
- 📊 **Real-time Metadata**: Fetch and display currently playing songs from API
- 🔄 **Dynamic Stream Management**: Add, remove, and switch between streams
- 📱 **Responsive Design**: Mobile, tablet, and desktop layouts
- 🎯 **Active Stream Indicator**: Visual feedback for currently playing stream
- 💾 **JSON Stream Configuration**: Easy stream management via `streams.json`
- 🔊 **Volume Control**: Dedicated volume slider in player bar
- ⏱️ **Progress Bar**: Visual playback progress with scrubbing
- 📐 **Design System Documentation**: Complete "Ethereal Broadcaster" design guidelines

### Technical Features
- **Vanilla JavaScript**: No dependencies required
- **Tailwind CSS**: Responsive utility-first styling
- **Material Design Icons**: Comprehensive icon library
- **CORS-Compatible**: Supports HTTP and HTTPS streams
- **Auto-metadata Refresh**: Updates every 30 seconds while playing
- **Graceful Fallbacks**: Works with or without metadata API

### Components
- Sidebar Navigation with home, library, and favorites
- Search Bar for stream discovery
- Hero Section with current artist/stream info
- Stream List with genre badges and quick actions
- Floating Player Bar with full controls
- Active Streams Panel
- Add Stream Modal
- Volume Control Panel

### Files
- `index.html` - Main application
- `streams.json` - 30 pre-configured Europe 2 streams
- `README.md` - User documentation
- `DESIGN.md` - Design system guidelines
- `package.json` - Project metadata
- `.gitignore` - Git configuration
- `CHANGELOG.md` - This file

## [Unreleased]

### Planned Features
- [ ] Local storage for user's custom stream list
- [ ] Stream metadata caching
- [ ] Equalizer with preset bands
- [ ] Recording/saving stream segments
- [ ] Stream quality selection
- [ ] Dark/Light theme toggle
- [ ] Export/import stream lists (JSON/M3U)
- [ ] Playlist creation and management
- [ ] Recently played history
- [ ] Stream favorites/bookmarks
- [ ] Share current playing on social media
- [ ] Mobile app (React Native/Flutter)
- [ ] Desktop app (Electron)
- [ ] Offline playback support
- [ ] Lyrics display integration
- [ ] Social listening with friends
- [ ] Audio analytics

### Performance Improvements
- [ ] Service Worker for offline support
- [ ] Cache strategy optimization
- [ ] Lazy loading for stream list
- [ ] WebWorker for metadata updates
- [ ] IndexedDB for stream history

### Accessibility
- [ ] ARIA labels for all interactive elements
- [ ] Keyboard navigation support
- [ ] Screen reader testing
- [ ] High contrast mode
- [ ] Focus management improvements

---

## Installation

### Prerequisites
- Modern web browser (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- No build process required

### Quick Start
```bash
git clone https://github.com/yourusername/streamlife.git
cd streamlife
python -m http.server 8000
# Visit http://localhost:8000
```

## Support & Contributing

For issues, feature requests, or contributions:
- Open an [Issue](https://github.com/yourusername/streamlife/issues)
- Submit a [Pull Request](https://github.com/yourusername/streamlife/pulls)
- Check [Contributing Guidelines](CONTRIBUTING.md)

## License

MIT License - See [LICENSE](LICENSE) file for details

## Credits

- **Design**: Inspired by Europe 1 and Europe 2 Radio UI
- **Icons**: [Google Material Symbols](https://fonts.google.com/icons)
- **Fonts**: [Google Fonts](https://fonts.google.com/)
- **CSS**: [Tailwind CSS](https://tailwindcss.com/)
- **Streams**: [RFM Network](https://www.rfm.fr/)

---

**Made with ♥ for radio enthusiasts and audio lovers everywhere.**
