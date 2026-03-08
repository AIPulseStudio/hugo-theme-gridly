# Hugo Theme Gridly

A modular, high-performance, and SEO-optimized Hugo theme designed for sports news and match schedules. Consolidated from 18+ live sports sites, **Gridly** offers extreme flexibility through parameterized layout variants and hero widgets.

## Features

- **🚀 Hugo Module Support**: Modern Hugo workflow for easy updates.
- **📱 Responsive Design**: Premium look on all devices.
- **🧩 Modular Layouts**: Choose from `grid`, `bento`, `featured`, or `list-sidebar`.
- **🎯 Dynamic Widgets**: Switch between `teams`, `match`, `stars`, and `page-header` hero sections.
- **🔍 SEO Optimized**: Built-in JSON-LD, OpenGraph, and semantic HTML5.
- **🎨 Parameterized Branding**: Full control over colors and logos via `hugo.toml`.

## Installation

Add this theme as a Hugo Module to your site:

```bash
hugo mod init github.com/yourusername/yoursite
hugo mod get github.com/AIPulseStudio/hugo-theme-gridly
```

And add it to your `hugo.toml`:

```toml
[module]
  [[module.imports]]
    path = "github.com/AIPulseStudio/hugo-theme-gridly"
```

## Configuration

### Global Settings

```toml
baseURL = 'https://example.com'
title = 'Sports News'

[params.colors]
  primary = '#004D98'
  secondary = '#EE324E'
  accent = '#FFD700'
  dark = '#1a1a2e'

[params.logo]
  text = "SN"
  title = "Sports"
  subtitle = "News"
```

### Layout Selection

Choose your home page layout variant:

```toml
[params.home]
  layout = 'grid' # Options: grid, bento, featured, list-sidebar
```

### Hero Widgets

Select a dynamic widget for your hero section:

```toml
[params.hero]
  widget = 'match' # Options: teams, match, stars, page-header
  badge = '🏆 LIVE MATCH'
  title = 'World Cup Finals'

[params.hero.match]
  home = 'Team A'
  away = 'Team B'
  score = '2 - 1'
  time = '85'
  venue = 'National Stadium'
```

## Content Structure

Ensure your posts are in the `content/posts/` directory. Each post can include metadata:

```markdown
---
title: "Match Analysis"
date: 2024-03-08
category: "Analysis"
images: ["/images/feature.webp"]
---
```

## License

Created by AIPulse Studio.
