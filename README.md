# Who Are the Nones?

An interactive guess-first activity about Americans with no religious affiliation, the religious “nones.” Students make five guesses (how many there are, how many are atheists, what they believe, how they differ by age, and whether the trend is still rising), then see the answers from Pew Research Center’s 2023–24 Religious Landscape Study. By Gwen Sharp.

**Live site:** https://gsharpokie.github.io/nones/

## What it does

- **Five guesses,** each followed by bars showing the answer and the student’s guess.
- **U.S. adults by religious identity:** Christian, other religions, atheist, agnostic, and “nothing in particular.”
- **All five answers** in one place.
- **The fuller picture:** the recent leveling off, why researchers still expect change (generational replacement), believing vs. belonging, and why different surveys give different numbers.
- **Discussion questions.**

## For instructors

To show all the answers without guessing, add `#answers` to the link: https://gsharpokie.github.io/nones/#answers

## Data

- Pew Research Center. 2025. *Decline of Christianity in the U.S. Has Slowed, May Have Leveled Off* (2023–24 Religious Landscape Study; 36,908 adults surveyed July 2023–March 2024). https://www.pewresearch.org/religion/2025/02/26/decline-of-christianity-in-the-us-has-slowed-may-have-leveled-off/
  - Unaffiliated: 16% (2007), 23% (2014), 29% (2023–24); atheist 5%, agnostic 6%, nothing in particular 19%.
  - Christian: 78% (2007), 71% (2014), 62% (2023–24); 60–64% each year 2019–2024.
  - Ages 18–24 vs. 74+: unaffiliated 43% vs. 13%; Christian 46% vs. 80%.
  - Belief in God or a universal spirit: all adults 83%; nothing in particular 69%; agnostics 43%; atheists 7% (“Religious and Spiritual Beliefs” chapter).
  - Unaffiliated 28–31% each year 2019–2024 in Pew’s National Public Opinion Reference Survey, and the GSS and Gallup comparisons and birth-cohort figures (Appendix C).
- Davie, Grace. 1994. *Religion in Britain since 1945: Believing without Belonging*. Blackwell.

## Editing

All five questions are in `const Q = [` near the top of the `<script>` section of `index.html`. The breakdown bar is `const LANDSCAPE`. “The fuller picture” is plain text in the page. Pew’s next Religious Landscape Study isn’t scheduled; its yearly National Public Opinion Reference Survey is the best source for updates.

## Turning on the site (one time)

Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose the **main** branch and the **/ (root)** folder, and select **Save**. Keep Issues turned on so the “Suggest a correction” link works.

## Accessibility

This site aims to meet [WCAG 2.1](https://www.w3.org/TR/WCAG21/) Level AA, so it works for people who use screen readers, keyboards, or screen magnification.

- All buttons, sliders, and links can be reached and used with a keyboard, and show a visible outline when selected.
- Charts have text descriptions, and many also have a data table or a slider that reads out each value.
- Text meets WCAG AA color contrast standards.
- Pages fit narrow phone screens without sideways scrolling.

I checked it in November 2026 with automated accessibility testing (axe-core) plus keyboard and small-screen checks. It hasn’t yet been tested by people who use screen readers every day, so there may be problems I haven’t caught. If something doesn’t work for you, please [let me know](https://github.com/gsharpokie/nones/issues/new).

## Author

Created by Gwen Sharp ([@gsharpokie](https://x.com/gsharpokie)).

## License

© 2026 Gwen Sharp. Licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): you may share and adapt it for noncommercial purposes with credit. See [LICENSE](LICENSE). The survey figures belong to Pew Research Center; this license covers the page’s design, text, and code.
