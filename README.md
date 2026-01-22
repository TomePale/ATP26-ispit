# ATP26 Ispit

## Sadržaj

- [User Experience Design](user_experience.md)
- [History](history.md)
- [Elements](elements.md)
  - Research
  - Visual Design
  - Information Architecture
  - Interaction Design
  - Usability
  - Accessibility
    - WCAG Compliance
  - Human-Computer Interaction
    - Getting Ready to Design
    - Design
    - User Research

---

## Dokumentacija projekta

- [LICENSE.md](LICENSE.md) - MIT Licenca
- [CHANGELOG.md](CHANGELOG.md) - Povijest promjena

---

Primjer JavaScript funkcije za praćenje korisničkog iskustva:

```javascript
// UX Event Tracker - GitHub Gist Example
// https://gist.github.com/

class UXTracker {
  constructor(userId) {
    this.userId = userId;
    this.events = [];
    this.sessionStart = Date.now();
  }

  trackEvent(eventName, metadata = {}) {
    const event = {
      name: eventName,
      timestamp: Date.now(),
      metadata: metadata
    };
    this.events.push(event);
    console.log(`Event tracked: ${eventName}`);
  }

  getSessionDuration() {
    return Date.now() - this.sessionStart;
  }
}

// Primjer korištenja
const tracker = new UXTracker('user123');
tracker.trackEvent('page_view', { page: '/home' });
tracker.trackEvent('button_click', { button: 'signup' });
```

---

## Galerija

![Universe](assets/universe.jpg)

*Slika: Vizualizacija kompleksnosti korisničkog iskustva*

---

## Izvori i reference

### Tekstualni izvori:
- [Wikipedia - User Experience Design](https://en.wikipedia.org/wiki/User_experience_design)
- [Nielsen Norman Group](https://www.nngroup.com/articles/definition-user-experience/)
- [Interaction Design Foundation](https://www.interaction-design.org/)

### Izvori slika:
- `mesh.png` - Lokalna datoteka iz assets foldera
- `universe.jpg` - Lokalna datoteka iz assets foldera

### Dodatna literatura:
- Norman, Donald (2013). *The Design of Everyday Things*
- Cooper, Alan (2014). *About Face: The Essentials of Interaction Design*

---

**Navigacija:** [History →](history.md) | [Elements →](elements.md)
