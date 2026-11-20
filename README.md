# Team Name: Team Calc

**Live site:** https://github.com/Babra-code/team-website.git
               

## Team
| Name          | Registration no. | GitHub username |
|---------------|------------------|-----------------|
|Babra Olweny   |COM/3436/26       |Babra-code       |
|Rihanna Achieng|COM/3455/26       |president-rihanna|

## Who drove each part
- Part 0, 2, 4: Babra Olweny
- Part 1, 3:Rihanna Achieng

## Personalisation
- Our colours:
- Projects we added:
- Extension challenge(s) completed:

## Reflection
1.​Lose: Native Tab focus / Enter or Space activation, and built-in button role/state (aria-expanded / aria-pressed).
​Affected: Keyboard-only users, screen-reader users, and assistive-technology users.
2.​What breaks: DOM queries and event listeners can fail because target elements don't exist yet.
​Why: A synchronous script in <head> blocks HTML parsing until it runs, before <body> elements are parsed into the DOM; defer lets parsing finish first.
3.​Risk: Visitor-supplied tags/scripts in titles can execute as HTML/JS (XSS) or break the page layout/DOM. textContent treats input as plain text.
4.Client-side JS can be bypassed (disabled JS, DevTools edits, or direct HTTP requests), so the server must validate to protect security, rules, and data integrity.
5.Home to Contact: Same origin (same scheme, host, and port), so they share localStorage.
​file:// vs. Live Server: Different origins (file:// vs. http://...), so browsers keep their localStorage separate.
6.​Duplicated: Navigation/header, footer (team name/year), and <head> links across pages.
​Problem & fix: Edits must be repeated across files, risking inconsistencies; avoid it using shared templates/partials or build/rendering scripts.