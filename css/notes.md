
# Campus Café Lab Notes

## HTTP observations — Task 1

| Observation | Result |
|---|---|
| Local URL | [Your localhost URL] |
| Request method | [Observed method] |
| Local status code | [Observed status] |
| Local server header | [Observed server header] |
| Missing page status | [Observed status] |

## CSS specificity — Task 4

An ID selector has higher specificity than a class selector, and a class selector has higher specificity than an element selector. When specificity is equal, the later matching rule normally wins.

## Selector examples — Task 4

| Selector | Purpose |
|---|---|
| `.card` | Selects elements with the card class |
| `#main` | Selects the element with the main ID |
| `a:hover` | Styles links while the pointer is over them |
| `input[required]` | Selects required input elements |
| `a[href^="http"]` | Selects links whose href starts with http |

## Bug log — Task 6

| # | What was wrong (file and line) | Which tool showed it | My fix |
|---|---|---|---|
| 1 | [Your finding] | [Tool] | [Fix] |
| 2 | [Your finding] | [Tool] | [Fix] |
| 3 | [Your finding] | [Tool] | [Fix] |
| 4 | [Your finding] | [Tool] | [Fix] |
| 5 | [Your finding] | [Tool] | [Fix] |
| 6 | [Your finding] | [Tool] | [Fix] |
| 7 | [Your finding] | [Tool] | [Fix] |
| 8 | [Your finding] | [Tool] | [Fix] |
| 9 | [Your finding] | [Tool] | [Fix] |
| 10 | [Your finding] | [Tool] | [Fix] |

## Live site observations — Task 7

1. **Localhost vs live site:** [Record the local and live protocols, server headers and Remote Address shown in DevTools.]

2. **HTTPS certificate:** [Record the certificate issuer and validity dates. Explain how HTTPS helps protect data in transit.]

3. **Saved orders:** Orders saved on localhost do not automatically appear on the live site because localStorage is separated by origin.

4. **Missing page:** [Record the status code and what the browser displayed for your missing-page request.]
