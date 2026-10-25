
# Campus Café — Lab 4 Notes

## HTTP observations (Lab 4, Task 1)

| Question | My answer |
|---|---|
| Request method for index.html | GET |
| Status code with Disable cache ticked | 200 OK |
| Status code on a normal reload | Record the value shown in DevTools |
| Status code for /nothing-here.html | 404 Not Found |
| Content-Type response header | Record the value shown in DevTools |
| Remote Address (IP and port) | Record the value shown in DevTools |
| Protocol in the address bar | http on localhost |

### Why is this address http and not https?

Localhost traffic stays on my own computer and does not travel across an external network. HTTPS is especially important when traffic travels across a network and needs encryption and authentication.

## Specificity experiment

The ID selector `#main p` overrides `.hero p` because ID selectors have higher specificity. Changing it to `main p` gives `.hero p` priority because class selectors have higher specificity than element selectors.

## Selectors I used

| Selector kind | Example from my CSS |
|---|---|
| Element | `body` |
| Class | `.hero` |
| ID | `#main` |
| Grouping | `h1, h2, h3` |
| Descendant | `.site-footer a` |
| Child (`>`) | `main > section` |
| Adjacent sibling (`+`) | `h1 + p` |
| Compound | `a.active` |
| Attribute | `a[href^="http"]` |
| Pseudo-class | `a:hover` |
| Pseudo-element | `a[href^="http"]::after` |

## Bug log

| Problem | Fix |
|---|---|
| CSS did not load | Corrected the stylesheet path to `css/styles.css`. |
| Hero text had the wrong color | Used `.hero h1, .hero p { color: #fff; }`. |
| External link arrow was missing | Used `a[href^="http"]::after`. |
| Form orders were not saved | Checked the form IDs, JavaScript path and localStorage code. |

## Live site observations (Lab 4, Task 7)

1. **Localhost vs live site:** Localhost uses HTTP and a local address. GitHub Pages uses HTTPS and a remote server. Record the actual server header and Remote Address shown in DevTools.
2. **Padlock and certificate:** The padlock indicates an encrypted HTTPS connection, and the certificate helps verify the site's identity. Plain HTTP traffic can potentially be read or changed by an attacker on the same Wi-Fi.
3. **Saved orders:** Orders saved on localhost do not appear on the live site because localStorage is separated by origin.
4. **Missing page:** The missing page should return `404 Not Found`. Record whether the response came from GitHub Pages or another server based on DevTools.
