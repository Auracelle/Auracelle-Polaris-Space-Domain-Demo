SECURITY.md
Auracelle Polaris · Security Policy & Responsible Disclosure

## Security Overview

Auracelle Polaris is a browser-based educational and research wargaming simulation 
designed for governance analysis and decision-making under pressure. While the 
simulation runs entirely client-side in your browser and does not collect, store, 
or transmit personal data, security and responsible use are important.

## Browser Security

Polaris runs entirely in your browser (client-side). It:

✓ Does NOT collect, store, or transmit user data
✓ Does NOT require authentication or login
✓ Does NOT use cookies or tracking technologies
✓ Does NOT require network connectivity after initial page load
✓ Does NOT execute external code or contact remote servers
✓ Does NOT use third-party libraries with external dependencies (except Google Fonts for typography)

However, please note:

- Your browser's JavaScript sandbox protects the system from most attacks
- If you are on a shared or untrusted device, consider browsing in a private/incognito window
- Keep your browser up to date with the latest security patches

## Responsible Use

Auracelle Polaris is intended for:

✓ Academic research on space governance
✓ Educational instruction in policy analysis and wargaming methodology
✓ Government and allied institution policy exploration
✓ Think tank and non-profit research
✓ Conference presentations and simulations

Prohibited uses:

✗ Commercial sale or licensing without explicit permission
✗ Reverse-engineering or attempting to extract proprietary methodology
✗ Unauthorized distribution or modification
✗ Use by adversarial or non-aligned states without written permission
✗ Misrepresentation of simulation outputs as real intelligence or predictions

See LICENSE.md for full terms of use.

## Reporting Security Issues

If you discover a security vulnerability or issue with Auracelle Polaris, please 
report it responsibly:

**DO NOT** post the vulnerability publicly or in GitHub Issues.

Instead, contact Grace-Alice Evans directly:

📧 Email: grace.evans@auracelle.ai
🔗 LinkedIn: https://www.linkedin.com/in/grace-alice-evans-5a9632a3

Please include:

1. Description of the security issue
2. Steps to reproduce (if applicable)
3. Potential impact
4. Suggested remediation (if you have one)

Grace-Alice will acknowledge receipt within 48 hours and work toward a resolution. 
We appreciate your responsible disclosure and will credit you in any security 
advisories if appropriate.

## Known Limitations

- Polaris is a decision-support tool, not a prediction engine. Simulation outputs 
  reflect programmed scenario logic and do not constitute intelligence or forecasts.
  
- The Agentic AI response logic is deterministic and rule-based, not machine-learned. 
  It models actor behavior based on game theory and governance principles, not real 
  data or advanced ML models.
  
- Scenarios are simplified representations of complex geopolitical situations. 
  Real-world space governance involves far more nuance and uncertainty than any 
  simulation can capture.
  
- Players should treat Polaris as a learning tool and decision-support aid, not as 
  a substitute for expert policy analysis or real intelligence.

## Data Privacy

Polaris does not collect, use, or share any user data. Your gameplay is:

- Stored only on your local device
- Not transmitted to Auracelle servers or third parties
- Not subject to any data retention or analytics
- Deleted when you close your browser (unless you manually save the page)

Your privacy is protected by your browser's sandbox and by our design commitment 
to avoid any data collection.

## Incident Response

In the unlikely event of a security incident affecting the Polaris repository or 
GitHub Pages deployment:

1. GitHub will notify repository administrators
2. Auracelle will investigate and publish a security advisory if necessary
3. Users will be directed to update or take action via the README and GitHub Releases

For real-time notifications, "Watch" the Polaris repository on GitHub.

## Dependency and Third-Party Code

Polaris uses the following external resources:

**Google Fonts (CSS)**:
- URL: https://fonts.googleapis.com/css2?family=Rajdhani:wght@400;500;600;700&family=Space+Grotesk:wght@400;500;600;700&family=Space+Mono:wght@400;700&display=swap
- Purpose: Typography only (no JavaScript execution or tracking)
- Privacy: See Google Fonts privacy policy

**No external JavaScript libraries** — Polaris is written in vanilla JavaScript and 
does not use jQuery, React, Vue, or other frameworks. This minimizes attack surface.

## Suggestions for Improvement

If you have suggestions for improving Polaris's security, privacy, or responsible 
use practices, please reach out:

📧 grace.evans@auracelle.ai

We welcome feedback on all aspects of the platform.

## Version & Last Updated

**Polaris Version**: 2.0  
**Security Policy Version**: 1.0  
**Last Updated**: June 2026

---

Thank you for using Auracelle Polaris responsibly.
