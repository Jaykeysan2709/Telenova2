# Talenova Design Guidelines

## Design Approach

**Reference-Based Approach**: Drawing inspiration from **Duolingo** (gamified learning), **Khan Academy Kids** (child-friendly educational content), and **Spotify** (content discovery and categorization), while infusing authentic African visual language.

**Core Design Principles**:
- **Cultural Authenticity**: Every element celebrates African heritage through patterns, symbols, and storytelling
- **Playful Learning**: Educational content feels like play, never like work
- **Age-Appropriate**: Clear, large, colorful elements optimized for young learners (4-13 years)
- **Joyful Discovery**: Each interaction reveals something new and delightful

---

## Typography

**Font Families**:
- **Primary (Headings)**: Fredoka or Baloo 2 (rounded, friendly, playful)
- **Secondary (Body)**: Inter or DM Sans (clean, highly readable for young readers)
- **Accent (Cultural)**: Use for story titles and special moments

**Hierarchy**:
- **Story Titles**: 2.5rem - 3rem, bold, extra letter-spacing for impact
- **Section Headers**: 1.75rem - 2rem, semibold
- **Body Text**: 1.125rem - 1.25rem, regular (larger than typical for children)
- **Buttons/CTAs**: 1rem - 1.125rem, medium weight

---

## Layout System

**Spacing Primitives**: Use Tailwind units of **2, 4, 6, 8, 12, and 16** for consistent rhythm
- Card padding: p-6
- Section spacing: py-12 to py-16
- Component gaps: gap-4 to gap-6
- Generous whitespace between learning modules

**Container Strategy**:
- Main content: max-w-6xl for immersive story reading
- Grid layouts: 2-3 columns on desktop, always single column on mobile
- Sidebar navigation: Fixed left sidebar (w-64) on desktop, bottom nav on mobile

---

## Component Library

### Navigation
- **Top Bar**: App logo (left), profile/parent access (right), points/badges display
- **Bottom Navigation (Mobile)**: Large icons for Stories, Games, Map, Profile (min-h-16, touch-friendly)
- **Sidebar (Desktop)**: Vertical navigation with icons + labels, collapsible story categories

### Story Cards
- Large, colorful cards with illustrated character previews
- Rounded corners (rounded-2xl) with subtle shadow
- Story title, region badge, language indicator, difficulty level (stars/age range)
- "Play Audio" button with waveform animation
- Hover: Gentle lift effect (translate-y-1)

### Content Display
- **Story Reader**: Full-screen immersive mode, large text (1.5rem), illustrated backgrounds, tap-to-advance
- **Flashcard Interface**: Flip animation, large centered text/images, swipe gestures
- **Quiz Components**: Multiple choice with vibrant answer buttons, celebration animations on correct answers
- **Cultural Map**: Interactive SVG map with pulsing markers, country cards slide in on click

### Game Elements
- **Score Displays**: Large, prominent with African-inspired number formatting
- **Badge System**: Collectible cowrie shells, cultural artifacts as unlockables
- **Progress Bars**: Thick (h-4), animated fills, tribal pattern overlays
- **Timer Elements**: Circular progress indicators with Adinkra symbol backgrounds

### Input Components
- **Buttons**: Extra large (h-12 to h-14), fully rounded (rounded-full), bold text
- **Text Inputs**: Larger size (text-lg), generous padding (py-4), friendly rounded borders
- **Toggle Switches**: Oversized for easy child interaction
- **Voice Recording**: Large microphone button with recording wave visualization

### Modals & Overlays
- **Story Selection Modal**: Full-screen overlay with story preview, auto-play audio sample
- **Achievement Popups**: Celebratory animations, confetti effects, cultural symbols
- **Parent Dashboard**: Distinct visual treatment (more sophisticated, data-focused)

---

## Visual Elements

### African Cultural Integration
- **Adinkra Symbols**: Use as decorative elements in corners, dividers, and backgrounds (subtle opacity)
- **Tribal Patterns**: Border treatments, card backgrounds (low opacity overlays)
- **Cowrie Shell Motif**: Currency/points system visualization
- **Geometric Patterns**: Inspired by Kente cloth, Ndebele art for section dividers

### Illustrations & Icons
- **Icon Library**: Heroicons for UI elements, supplement with custom African-themed icons
- **Character Illustrations**: Vibrant, cartoon-style African characters with diverse representation
- **Story Thumbnails**: Hand-drawn aesthetic with bold outlines and flat colors
- **Loading States**: Animated African wildlife characters (elephant, lion, tortoise)

### Interactive Feedback
- **Button Presses**: Gentle scale animation (scale-95), sound effects (African drum hits)
- **Success States**: Confetti, sparkles, celebratory African music snippets
- **Transitions**: Smooth page transitions (300ms), slide/fade effects
- **Micro-interactions**: Heartbeat animations for favorites, bounce for new unlocks

---

## Images

**Hero Section** (Home/Landing):
- Large illustrated scene featuring diverse African children reading/playing together
- Background: Savanna sunset or baobab tree with storybook elements floating around
- Placement: Full-width hero (min-h-96), overlay with blurred-background CTA buttons

**Story Library**:
- Each story category has distinct header image (folklore creatures, landscapes, cultural scenes)
- Thumbnail images for every story card (character portraits, key story moments)

**Cultural Map**:
- Illustrated map of Africa with artistic styling (not realistic, cartoon-like)
- Country-specific imagery appears on selection (traditional clothing, landmarks, animals)

**Achievement Gallery**:
- Badge/reward images using African artifacts (masks, drums, fabrics)
- Progress milestone illustrations showing cultural milestones

**Parent Dashboard**:
- Header image with parent + child reading together in warm setting

---

## Age-Specific Considerations

**Ages 4-7**:
- Extra large buttons and touch targets (min 60px)
- Heavy use of images and icons over text
- Bright, high-contrast elements
- Simple navigation with picture-based categories

**Ages 8-10**:
- Balance of text and visuals
- More detailed story cards with longer descriptions
- Introduction of point systems and leaderboards
- Multi-step game mechanics

**Ages 11-13**:
- More sophisticated UI with deeper content hierarchy
- Reading-heavy sections with chapter navigation
- Advanced language features (sentence construction)
- Community features and story creation tools

---

## Accessibility

- Minimum touch targets: 48px × 48px (WCAG AAA)
- Text-to-speech integration for all story content
- High contrast mode toggle in settings
- Keyboard navigation for all interactive elements
- Audio alternatives for visual content
- Dyslexia-friendly font options (OpenDyslexic available)
- Screen reader optimization for educational content

---

**Design Vision**: AfroTales should feel like stepping into a vibrant, magical storybook where African culture comes alive through every interaction. The interface is a celebration—colorful, warm, inviting, and deeply rooted in African heritage while being thoroughly modern and delightful for young learners.