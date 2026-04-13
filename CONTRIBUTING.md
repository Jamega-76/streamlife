# Contributing to StreamLife

Thank you for your interest in contributing to StreamLife! We welcome contributions from everyone, whether it's code, design suggestions, documentation, or bug reports.

## Code of Conduct

- Be respectful and inclusive
- Focus on what's best for the community
- Show empathy to other community members

## Getting Started

### Prerequisites
- Git
- Basic knowledge of HTML, CSS, and JavaScript
- A code editor (VS Code, Sublime, etc.)
- A modern web browser

### Fork & Clone
```bash
# Fork the repository on GitHub
git clone https://github.com/yourusername/streamlife.git
cd streamlife
```

### Set Up Development Environment
```bash
# No build process needed!
# Simply run a local server
python -m http.server 8000

# Visit http://localhost:8000 in your browser
```

## Development Workflow

### 1. Create a Feature Branch
```bash
git checkout -b feature/your-feature-name
# or for bug fixes:
git checkout -b fix/bug-description
```

### 2. Make Your Changes

Follow these guidelines:

#### Code Style
- Use consistent indentation (2 spaces)
- Use meaningful variable and function names
- Keep functions focused and small
- Add comments for complex logic

#### HTML
```html
<!-- Good: semantic, clear -->
<button onclick="playStream(0)" class="primary-button">
  <span class="material-symbols-outlined">play_arrow</span>
  Play
</button>

<!-- Avoid: unclear, no semantics -->
<div onclick="foo()" class="btn">Play</div>
```

#### CSS
- Use Tailwind classes first
- Only add custom CSS when necessary
- Follow the design system tokens
- Use CSS variables for colors when overriding

#### JavaScript
```javascript
// Good: clear function names, proper scoping
function playStream(index) {
  const stream = streams[index];
  togglePlayback();
}

// Avoid: unclear names, global variables
function p(i) {
  window.s = streams[i];
  toggle();
}
```

### 3. Test Your Changes

- Test in multiple browsers (Chrome, Firefox, Safari, Edge)
- Test on different screen sizes (mobile, tablet, desktop)
- Verify accessibility (keyboard navigation, screen readers)
- Check metadata loading works correctly
- Ensure no console errors

### 4. Update Documentation

If your changes affect functionality:
- Update `README.md` if needed
- Update `DESIGN.md` for design changes
- Add entry to `CHANGELOG.md` under [Unreleased]
- Update code comments

### 5. Commit Your Changes

```bash
git add .
git commit -m "feat: add feature description" 

# Commit message format:
# feat: add new feature
# fix: fix a bug
# docs: update documentation
# style: improve code style
# refactor: restructure code
# test: add/update tests
```

### 6. Push & Create Pull Request

```bash
git push origin feature/your-feature-name
```

Then go to GitHub and create a Pull Request with:
- Clear title describing the change
- Description of what changed and why
- Screenshots for UI changes
- Link to related issues (if any)

## Pull Request Guidelines

### Before Submitting
- [ ] Code follows project style guide
- [ ] Changes tested in multiple browsers
- [ ] No console errors or warnings
- [ ] Comments added for complex code
- [ ] Documentation updated

### PR Description Template
```markdown
## Description
Brief explanation of the changes.

## Type of Change
- [ ] New feature
- [ ] Bug fix
- [ ] Documentation update
- [ ] Design improvement

## How to Test
Steps to verify the changes:
1. ...
2. ...
3. ...

## Screenshots (if applicable)
[Add screenshots for UI changes]

## Checklist
- [ ] Changes tested
- [ ] Documentation updated
- [ ] No breaking changes
- [ ] Code follows style guide
```

## Issue Guidelines

### Reporting Bugs

**Title**: Clear, concise description
**Description**:
```
**Describe the bug**
[Clear description of what's broken]

**Steps to Reproduce**
1. Go to...
2. Click...
3. See error...

**Expected Behavior**
[What should happen]

**Actual Behavior**
[What actually happens]

**Environment**
- Browser: [e.g., Chrome 125]
- OS: [e.g., macOS 14.0]
- Device: [e.g., MacBook Pro]

**Screenshots**
[If applicable]

**Additional Context**
[Any other relevant info]
```

### Feature Requests

**Title**: Clear description of feature

**Description**:
```
**Is your feature request related to a problem?**
[Describe the problem]

**Describe the solution you'd like**
[How should it work]

**Describe Alternatives**
[Other approaches]

**Additional Context**
[Why this matters]
```

## Project Structure

```
streamlife/
├── index.html          # Main application
├── streams.json        # Stream configuration
├── README.md           # User guide
├── DESIGN.md           # Design system
├── CHANGELOG.md        # Version history
├── CONTRIBUTING.md     # This file
├── LICENSE             # MIT License
└── package.json        # Project metadata
```

## Key Areas for Contribution

### High Priority
- [ ] Audio playback implementation
- [ ] Actual metadata parsing from API
- [ ] Cross-browser audio compatibility
- [ ] Mobile responsiveness fixes
- [ ] Accessibility improvements

### Medium Priority
- [ ] Stream search/filter functionality
- [ ] Favorite streams persistence
- [ ] Stream history tracking
- [ ] Keyboard shortcuts
- [ ] Dark/light theme toggle

### Low Priority
- [ ] UI animations
- [ ] Additional stream sources
- [ ] Documentation improvements
- [ ] Localization/i18n

## Design System Compliance

When making UI changes, ensure:
- Colors follow `streams.json` or DESIGN.md color tokens
- Spacing uses Tailwind scale (8, 12, 16, 24, 32, 48...)
- Rounded corners use design tokens (sm, md, lg, xl, full)
- No hardcoded colors - use Tailwind classes
- Glassmorphic elements use `glass-panel` class
- Icons use Material Symbols Outlined

## Performance Guidelines

- Keep bundle size minimal (no external JS dependencies required)
- Use efficient selectors and avoid redundant DOM queries
- Cache frequently accessed DOM elements
- Use event delegation for dynamic content
- Minimize metadata API calls (max 30s intervals)

## Documentation

- Use clear, concise language
- Include code examples
- Update README for user-facing changes
- Update DESIGN.md for visual/interaction changes
- Keep docs in sync with code

## Getting Help

- Check existing issues/PRs for similar requests
- Ask questions in GitHub discussions
- Review DESIGN.md for design decisions
- Check CHANGELOG.md for recent changes

## Review Process

1. **Automated Checks**: Basic validation
2. **Code Review**: Maintainer review of changes
3. **Testing**: Verification in multiple browsers
4. **Feedback**: Comments and suggestions
5. **Merge**: Once approved!

## After Merge

Your contribution will be:
- Merged to the main branch
- Included in the next release
- Credited in CHANGELOG.md
- Mentioned in community highlights

## Questions?

- Open a GitHub Issue
- Start a GitHub Discussion
- Email the maintainers

---

**Thank you for making StreamLife better!** 🎙️✨
