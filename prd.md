# Product Requirements Document: Seattle Kraken Second Screen Companion App (Prototype)

## Document Information
- **Product Name:** Kraken Companion (Working Title)
- **Version:** 0.1 (Prototype)
- **Date:** March 11, 2026
- **Document Owner:** [Your Name]
- **Status:** Draft

---

## 1. Executive Summary

The Kraken Companion app is a second-screen mobile experience designed to help first-time hockey fans and newcomers understand the game in real-time during Seattle Kraken home games. When key game events occur (penalties, offsides, icing, etc.), the app delivers bite-sized, 10-second animated video explainers that educate without detracting from the live experience.

**This is a prototype** intended to demonstrate core functionality and user experience, not a fully functional production app.

---

## 2. Problem Statement

First-time hockey attendees often feel confused or left out when game stoppages occur due to rules they don't understand (offsides, icing, penalties, etc.). This creates a barrier to engagement and can diminish the live game experience for newcomers.

---

## 3. Goals & Objectives

### Primary Goals
- Educate first-time hockey fans about game rules in real-time
- Enhance the in-arena experience without distracting from live action
- Create brand affinity with the Seattle Kraken through helpful, accessible content

### Success Metrics (Prototype)
- User engagement with video explainers
- Thumbs up/down feedback ratio
- Time spent viewing videos (target: <10 seconds per video)

---

## 4. Target Audience

**Primary Persona: "Sarah the First-Timer"**
- Age: 25-40
- Attending first or second Kraken game
- Limited hockey knowledge
- Wants to understand and enjoy the game
- Mobile-savvy, comfortable using apps during events

---

## 5. User Story

> Sarah is attending her first Seattle Kraken game at Climate Pledge Arena. The referee blows the whistle and signals offsides. Sarah doesn't know what that means. She opens the Kraken Companion app on her phone, where a simple 10-second animated video explains offsides using a bird's-eye view of the rink with text overlays. The video pauses at key moments for clarity. After watching, Sarah taps "thumbs up" to indicate the video was helpful. She now understands the call and can return her attention to the ice.

---

## 6. Core Features (Prototype Scope)

### 6.1 Real-Time Event Detection (Simulated)
**Description:** The prototype will simulate real-time game event detection. In a production app, this would integrate with game data feeds.

**Prototype Behavior:**
- Manual trigger or timer-based simulation of common game events
- Events include: Offsides, Icing, Penalty (High-Sticking), Goal Review, Face-Off

### 6.2 Video Explainer Library
**Description:** Short, animated video explainers for common hockey rules and situations.

**Specifications:**
- **Duration:** Maximum 10 seconds per video
- **Style:** Simple line animations, bird's-eye view of hockey rink
- **Animation:** Minimal, clean motion graphics
- **Text Overlays:** Clear, concise explanations
- **Pausing:** Videos pause at 2-3 key moments for emphasis
- **Color Palette:** Seattle Kraken brand colors
  - **Deep Sea Blue:** #001628 (primary background)
  - **Ice Blue:** #99D9D9 (primary accent)
  - **Shadow Blue:** #355464 (secondary)
  - **Boundless Blue:** #001F5B (secondary)
  - **Red Alert:** #C8102E (highlights/alerts)

**Prototype Videos (Minimum 3):**
1. Offsides
2. Icing
3. High-Sticking Penalty

### 6.3 User Feedback Mechanism
**Description:** Simple thumbs up/down feedback at the end of each video.

**Specifications:**
- Appears immediately after video completes
- Two options: 👍 Thumbs Up | 👎 Thumbs Down
- Single tap to submit
- Brief confirmation message: "Thanks for your feedback!"
- Feedback stored (simulated in prototype)

### 6.4 Mobile-First UI
**Description:** Clean, intuitive interface optimized for mobile viewing in low-light arena conditions.

**Specifications:**
- Dark mode default (Deep Sea Blue background)
- High contrast text (Ice Blue and white)
- Large, tappable buttons
- Minimal navigation
- Quick access to video library

---

## 7. User Flow

```
1. User opens Kraken Companion app
   ↓
2. App displays "Listening for game events..." (simulated)
   ↓
3. Game event occurs (e.g., Offsides)
   ↓
4. Notification appears: "What just happened? Tap to learn about Offsides"
   ↓
5. User taps notification
   ↓
6. 10-second animated video plays
   ↓
7. Video pauses at key moments with text overlays
   ↓
8. Video completes
   ↓
9. Feedback prompt appears: "Was this helpful?"
   ↓
10. User taps 👍 or 👎
    ↓
11. Confirmation: "Thanks for your feedback!"
    ↓
12. Return to listening state
```

---

## 8. Design Specifications

### 8.1 Color Palette
Based on Seattle Kraken brand guidelines:

| Color Name | Hex Code | Usage |
|------------|----------|-------|
| Deep Sea Blue | #001628 | Primary background, headers |
| Ice Blue | #99D9D9 | Primary accent, interactive elements |
| Shadow Blue | #355464 | Secondary backgrounds, cards |
| Boundless Blue | #001F5B | Secondary accent |
| Red Alert | #C8102E | Notifications, penalties |
| White | #FFFFFF | Primary text on dark backgrounds |

### 8.2 Typography
- **Headings:** Tungsten Bold (Kraken brand font)
- **Body Text:** Roboto Regular (clean, readable)
- **Font Sizes:**
  - H1: 24px
  - H2: 18px
  - Body: 16px
  - Small: 14px

### 8.3 Video Animation Style
- **View:** Bird's-eye view of hockey rink
- **Elements:** Simple line drawings (rink, players, puck)
- **Player Representation:** Colored circles or simple stick figures
- **Motion:** Smooth, minimal animation
- **Pauses:** 2-3 strategic pauses with text overlays
- **Text Style:** Sans-serif, high contrast, large enough to read quickly

---

## 9. Technical Requirements (Prototype)

### 9.1 Platform
- **Primary:** iOS (iPhone)
- **Secondary:** Android (optional for prototype)

### 9.2 Technology Stack (Suggested)
- **Framework:** React Native or Flutter (for cross-platform prototype)
- **Video Playback:** Native video player with custom controls
- **Animation:** Pre-rendered MP4 videos or After Effects exports
- **State Management:** Simple local state (no backend required for prototype)

### 9.3 Assets Required
- 3-5 animated video explainers (MP4 format, 1080x1920 vertical or 1920x1080 horizontal)
- Kraken logo and branding assets
- UI icons (thumbs up/down, play/pause, etc.)

### 9.4 Data Storage (Prototype)
- Local storage only
- No user accounts or authentication required
- Feedback data stored locally (not transmitted)

---

## 10. Out of Scope (For Prototype)

The following features are **NOT** included in this prototype but may be considered for future iterations:

- Live game data integration
- Push notifications
- User accounts and profiles
- Social sharing features
- Multiple language support
- Accessibility features (screen reader support, captions)
- Analytics dashboard
- Content management system for videos
- Offline mode
- Apple Watch or wearable integration

---

## 11. Success Criteria (Prototype)

This prototype will be considered successful if it demonstrates:

1. ✅ Clear, understandable video explainers that educate users in <10 seconds
2. ✅ Intuitive user flow from event trigger to video playback to feedback
3. ✅ On-brand visual design using Kraken colors and style
4. ✅ Positive user feedback during testing (>70% thumbs up)
5. ✅ Minimal distraction from live game experience

---

## 12. Timeline & Milestones

| Milestone | Deliverable | Target Date |
|-----------|-------------|-------------|
| Kickoff | PRD Approval | Week 1 |
| Design | UI/UX Mockups | Week 2 |
| Content | 3 Video Explainers | Week 3 |
| Development | Functional Prototype | Week 4-5 |
| Testing | User Testing & Feedback | Week 6 |
| Delivery | Final Prototype Demo | Week 7 |

---

## 13. Risks & Mitigations

| Risk | Impact | Mitigation |
|------|--------|------------|
| Video production takes longer than expected | High | Start with 1-2 videos; add more iteratively |
| Users find videos too long or distracting | High | Strict 10-second limit; test with real users |
| Prototype doesn't feel "real" enough | Medium | Use high-quality animations and polished UI |
| Brand guidelines not followed | Medium | Regular check-ins with Kraken brand team |

---

## 14. Appendix

### 14.1 Example Video Script: Offsides

**Duration:** 10 seconds

**Visual Sequence:**
1. [0-2s] Bird's-eye view of hockey rink. Offensive team (Ice Blue) attacking.
2. [2-4s] **PAUSE** - Text overlay: "Offsides happens when an attacking player crosses the blue line before the puck"
3. [4-6s] Animation shows player (red circle) crossing blue line ahead of puck
4. [6-8s] **PAUSE** - Text overlay: "Play stops and face-off moves outside the zone"
5. [8-10s] Animation shows face-off dot outside blue line. **END**

### 14.2 Wireframe Descriptions

**Home Screen:**
- Kraken logo at top
- "Listening for game events..." status indicator
- Button: "Browse All Rules" (leads to video library)
- Dark background (Deep Sea Blue)

**Video Player Screen:**
- Full-screen video player
- Minimal controls (play/pause only)
- Progress bar at bottom
- Text overlays appear on video

**Feedback Screen:**
- "Was this helpful?" heading
- Large 👍 and 👎 buttons (Ice Blue accent)
- "Thanks for your feedback!" confirmation
- "Back to Game" button

---

## 15. Approval & Sign-Off

| Role | Name | Signature | Date |
|------|------|-----------|------|
| Product Owner | | | |
| Design Lead | | | |
| Engineering Lead | | | |
| Stakeholder | | | |

---

**End of Document**