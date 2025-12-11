---
layout: page
title: Accessibility
permalink: /accessibility/
---

# Accessibility at vlrb

Video messaging should be for everyone. That's not just something we say—it's how we build vlrb. From the first line of code, we've designed with accessibility in mind because we believe the joy of connecting through video shouldn't depend on how you see, hear, move, or interact with your phone.

Whether you use VoiceOver, prefer larger text, or need reduced motion, vlrb is built to work beautifully for you.

---

## Our Philosophy

Accessibility isn't a feature we add later. It's not a compliance checkbox. It's how we build from the start.

We follow the Seven Principles of Universal Design because we believe accessible design makes vlrb better for everyone. When we make the app easier to use for someone with a disability, we often make it easier for everyone. Larger touch targets help people with motor differences—and also help when you're recording one-handed while holding a cup of tea. Clear labels help screen reader users—and also help everyone understand what a button does.

Our goal isn't just to meet standards. Our goal is delight. We want the accessible experience to be just as warm and joyful as any other experience of vlrb.

---

## VoiceOver Support

vlrb has comprehensive VoiceOver support throughout the entire app. We don't just add labels—we think carefully about what information you need and when you need it.

**Every element has meaning.** All interactive elements have accessibility labels that describe what they are and what they do. Hints tell you what will happen when you tap. Nothing is left unlabeled or mysterious.

**Recording is fully accessible.** When you're recording, vlrb keeps you informed:
- "Recording started" confirms you're capturing
- Time warnings at 60 seconds, 30 seconds, and 10 seconds remaining
- A countdown from 5 to 1 as you approach the limit
- "Recording stopped" confirms completion
- Buttons are clearly labeled: "Record video," "Stop recording," "Pause," "Resume"

**Navigation flows naturally.** Chat navigation announces contact names, online status, unread message counts, and timestamps. Related information—like a contact's name and their status—is grouped into single, meaningful announcements so you don't have to piece things together.

**Playback keeps you informed.** Video playback announces play/pause states and progress. You always know where you are and what's happening.

**Security you can hear.** When you send a message, vlrb announces "Message is end-to-end encrypted" so you know your moments are protected.

---

## Dynamic Type

All text in vlrb scales with your iOS text size preferences. We use Apple's dynamic text styles throughout—no fixed sizes that ignore your settings.

Whether you prefer extra small text or accessibility extra extra extra large, vlrb adapts. Our custom fonts (the warm serif for Cozy theme, the friendly rounded type for Modern) all scale properly. Nothing gets clipped or hidden. The app remains usable and beautiful at any size.

---

## Reduced Motion

If you have vestibular disorders or motion sensitivity, vlrb has you covered. We respect the iOS "Reduce Motion" setting throughout the entire app.

When you enable Reduce Motion:
- All animations are disabled
- Transitions become instant rather than animated
- No sudden movements or disorienting effects
- Button animations, loading indicators, and page transitions all adapt

We built a custom motion preference system that checks your setting before every animation. Consistency matters.

---

## Color and Contrast

We've tested all text and interface elements across all four theme variants—Cozy Light, Cozy Dark, Modern Light, and Modern Dark—to ensure they meet color contrast standards.

**Text is readable.** All body text meets or exceeds a 4.5:1 contrast ratio. Large text and interface components maintain at least 3:1 contrast.

**Video overlays work on any content.** When text appears over video, we use high-contrast white text on a semi-transparent dark background, so you can read captions and controls no matter what's in the video.

**Color isn't the only signal.** We never rely on color alone to convey information. Status indicators, error states, and interactive elements always have additional cues beyond just color.

---

## Touch Targets

We've made sure all interactive elements are easy to tap, even if you have motor differences or are just in a hurry.

- **Record and Stop buttons**: 70 points—well above the recommended minimum
- **Navigation buttons**: 44 points or larger, with adequate spacing between them
- **Tab bar items**: Standard 44-point targets

No tiny buttons, no frustrating missed taps.

---

## Haptic Feedback

vlrb uses thoughtful haptic feedback to provide confirmation you can feel, not just see or hear.

**During recording:**
- Two quick taps confirm recording has started
- A success vibration confirms completion
- Gentle pulses at 30 seconds, increasing urgency at 10 seconds
- Distinct taps for each second from 5 to 1

**During playback:**
- Different patterns distinguish pause from resume

**For errors:**
- A clear error haptic when something goes wrong

Haptics follow your iOS preferences and won't surprise you if you've turned them off.

---

## Keyboard Navigation

If you use an external keyboard with your iPhone or iPad, vlrb supports proper keyboard navigation. Focus states are visible and logical, tab order follows visual hierarchy, and text fields behave as you'd expect.

---

## Switch Control

vlrb works with iOS Switch Control. Interactive elements have proper accessibility traits, the recording button is marked as starting a media session, and selection states are properly announced. We've marked headers for easy navigation so you can move through the app efficiently.

---

## Bold Text

When Bold Text is enabled in iOS settings, all text in vlrb respects your preference. Font weights scale appropriately and text remains readable and properly weighted.

---

## Theme Options

vlrb offers two themes, each designed with accessibility in mind:

**Cozy Theme** uses warm colors with a serif font, providing a classic, comfortable feel with strong contrast.

**Modern Theme** offers a clean design with rounded fonts and equally strong contrast.

Both themes are available in light and dark mode. All color combinations have been tested for accessibility compliance. Semantic colors—success, error, warning—are consistent and distinguishable across all themes.

---

## How We Test

We maintain a comprehensive accessibility test suite with over 700 lines of automated tests. Every build is checked for:

- Dynamic Type scaling at every size
- Reduced Motion preference handling
- Unique accessibility identifiers
- Color contrast compliance
- Touch target size requirements
- Complete VoiceOver labels
- Animation accessibility

We also test manually with VoiceOver, Switch Control, and various accessibility settings. Automated tests catch regressions, but human testing ensures the experience feels right.

---

## Coming Soon

We're actively working on these accessibility features:

**Closed captions for videos.** Automatic speech-to-text captioning for video messages, generated on-device to protect your privacy. No audio leaves your phone during transcription.

**Caption editing.** Review and correct auto-generated captions before sending, so your message comes across exactly as you intend.

**Caption customization.** Adjust font size, background opacity, and position of captions during playback to match your preferences.

---

## We're Not Done

Accessibility isn't a checkbox we tick and move on from—it's a continuous commitment. We're always looking for ways to make vlrb work better for more people.

If something isn't working for you, we want to know. Your experience matters to us, and your feedback directly shapes how we improve.

**Found an accessibility barrier?** Please reach out at {{ site.support_email }}. Tell us what happened and how it affected you. We read every message and take accessibility feedback seriously.

---

*vlrb – video blurbs for the people you love, designed for everyone.*
