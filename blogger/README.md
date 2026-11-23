# Blogger theme

Retro mono look for [dradoaica.blogspot.com](https://dradoaica.blogspot.com).

The design is inspired by [AprilNEA](https://github.com/AprilNEA)'s site, [aprilnea.me](https://aprilnea.me/en); the
blog footer credits it too.

[theme.xml](theme.xml) is the stock Blogger "Essential" theme with two additions, so the theme's widgets and scripts
stay untouched:

- a `<link>` above `<b:skin>` that loads the JetBrains Mono font
- a block of overrides at the end of the skin, starting at the `Retro mono look` comment

The settings blocks of the two hidden AdSense widgets are removed, because Blogger rejects them on upload.

## Install

Back up first: Blogger → Theme → ▾ next to Customize → Backup.

Either restore the theme: Theme → ▾ → Restore → upload [theme.xml](theme.xml).
Or paste it: Theme → ▾ → Edit HTML, select everything, replace it with the content of [theme.xml](theme.xml), and save.

To change the look, edit the overrides block at the end of the skin in `theme.xml`. Its colors are CSS variables at the
top of the block, with a second set for dark mode. By default the blog follows the reader's system setting; a switch
in the header, next to search, cycles system → light → dark and remembers the choice in the reader's browser.

## Pages

[about_me.html](about_me.html) and [projects.html](projects.html) are the bodies of the "About me" and "Projects"
pages. Paste each into the page editor in HTML view (Blogger → Pages).
