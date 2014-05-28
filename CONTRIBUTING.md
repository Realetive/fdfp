# Требования

Пожалуйста, потратьте несколько минут, чтобы ознакомиться с этим документом, регламентирующим процессы совместной разработки.

Следующее руководство поясняет такие моменты как использование трекера, оформление кода. Соблюдение этих условий гарантирует продуктивное развитие проекта, повышает производительность и помогает избежать конфликтов.

## Использование трекера

[Трекер](https://github.com/Realetive/fdfp/issues) является приоритетным способом оповещений о [найденных ошибках](#отчёт-об-ошибках), [пожеланиях по улучшению](#пожелания-по-улучшению) и [запросов на включение](#запрос-на-включение) (сделанных вами изменений), но, пожалуйста, придерживайтесь следующих принципов:

* Пожалуйста, **НЕ** используйте трекер для личных вопросов касательно использования, например, Twitter Bootstrap или MODx. Для этого есть специализированнные ресурсы, типа Stack Overflow (по тегам [`twitter-bootstrap-3`](http://stackoverflow.com/questions/tagged/twitter-bootstrap-3), [`modx-revolution`](http://stackoverflow.com/questions/tagged/modx-revolution) или клуб [MODx Санкт-Петербург](README.md#Сообщество), которые являются более ориентированными для этого.

* Пожалуйста, **НЕ** разводите холивары и не тролльте друг друга. Придерживайтесь теме обсуждения и оставляйте ваше мнение при себе.

* Пожалуйста, **НЕ** создавайте обращения на трекере касательно ошибок и проблем сторонних продуктов, используемых в проекте. Используйте соответствующие ресурсы, указанные в первоисточнике.

## Отчёт об ошибках

A bug is a _demonstrable problem_ that is caused by the code in the repository.
Good bug reports are extremely helpful, so thanks!

Guidelines for bug reports:

1. **Use the GitHub issue search** &mdash; check if the issue has already been
   reported.

2. **Check if the issue has been fixed** &mdash; try to reproduce it using the
   latest `master` or development branch in the repository.

3. **Isolate the problem** &mdash; ideally create a [reduced test
   case](http://css-tricks.com/6263-reduced-test-cases/) and a live example.
   [This JS Bin](http://jsbin.com/EBAwOkOK/1) is a helpful template.


A good bug report shouldn't leave others needing to chase you up for more
information. Please try to be as detailed as possible in your report. What is
your environment? What steps will reproduce the issue? What browser(s) and OS
experience the problem? Do other browsers show the bug differently? What
would you expect to be the outcome? All these details will help people to fix
any potential bugs.

Example:

> Short and descriptive example bug report title
>
> A summary of the issue and the browser/OS environment in which it occurs. If
> suitable, include the steps required to reproduce the bug.
>
> 1. This is the first step
> 2. This is the second step
> 3. Further steps, etc.
>
> `<url>` - a link to the reduced test case
>
> Any other information you want to share that is relevant to the issue being
> reported. This might include the lines of code that you have identified as
> causing the bug, and potential solutions (and your opinions on their
> merits).


## Пожелания по улучшению

Feature requests are welcome. But take a moment to find out whether your idea fits with the scope and aims of the project. It's up to *you* to make a strong case to convince the project's developers of the merits of this feature. Please provide as much detail and context as possible.


## Запросы на включение

Good pull requests—patches, improvements, new features—are a fantastic
help. They should remain focused in scope and avoid containing unrelated
commits.

**Please ask first** before embarking on any significant pull request (e.g.
implementing features, refactoring code, porting to a different language),
otherwise you risk spending a lot of time working on something that the
project's developers might not want to merge into the project.

Please adhere to the [coding guidelines](#code-guidelines) used throughout the
project (indentation, accurate comments, etc.) and any other requirements
(such as test coverage).

Adhering to the following process is the best way to get your work
included in the project:

1. [Fork](http://help.github.com/fork-a-repo/) the project, clone your fork,
   and configure the remotes:

   ```bash
   # Clone your fork of the repo into the current directory
   git clone https://github.com/<your-username>/bootstrap.git
   # Navigate to the newly cloned directory
   cd bootstrap
   # Assign the original repo to a remote called "upstream"
   git remote add upstream https://github.com/twbs/bootstrap.git
   ```

2. If you cloned a while ago, get the latest changes from upstream:

   ```bash
   git checkout master
   git pull upstream master
   ```

3. Create a new topic branch (off the main project development branch) to
   contain your feature, change, or fix:

   ```bash
   git checkout -b <topic-branch-name>
   ```

4. Commit your changes in logical chunks. Please adhere to these [git commit
   message guidelines](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)
   or your code is unlikely be merged into the main project. Use Git's
   [interactive rebase](https://help.github.com/articles/interactive-rebase)
   feature to tidy up your commits before making them public.

5. Locally merge (or rebase) the upstream development branch into your topic branch:

   ```bash
   git pull [--rebase] upstream master
   ```

6. Push your topic branch up to your fork:

   ```bash
   git push origin <topic-branch-name>
   ```

7. [Open a Pull Request](https://help.github.com/articles/using-pull-requests/)
    with a clear title and description against the `master` branch.

**ПРИМЕЧАНИЕ**: By submitting a patch, you agree to allow the project owners to license your work under the terms of the [MIT License](LICENSE.md).

## Code guidelines

### HTML

- Два пробела для отступа, никаких табуляций.
- Двойные кавычки для аттрибутов, никаких одиночных кавычек.
- Всегда используйте правильный отступ.
- Используйте теги и элементы, соответветствующии декларации HTML5 (например, «самозакрывающиеся» одиночные теги).
- Используйте [CDN-хостинги](http://ru.wikipedia.org/wiki/Content_Delivery_Network) для сторонних JavaScript-библиотек, если это возможно. Также, сохраняйте протокол http или https в URL для html-шаблонов вёрстки — это позволит просматривать их локально.
- Use [WAI-ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA) attributes in documentation examples to promote accessibility.

### CSS

- CSS changes must be done in `.less` files first, never just in the compiled `.css` files.
- Adhere to the [CSS property order](http://markdotto.com/2011/11/29/css-property-order/).
- Multiple-line approach (one property and value per line).
- Always a space after a property's colon (e.g., `display: block;` and not `display:block;`).
- End all lines with a semi-colon.
- For multiple, comma-separated selectors, place each selector on its own line.
- Don't add vendor prefixed properties to their unprefixed counterparts (e.g., only `box-sizing` and not also include `-webkit-box-sizing`), as this is done automagically at build time.
- Attribute selectors, like `input[type="text"]` should always wrap the attribute's value in double quotes, for consistency and safety (see this [blog post on unquoted attribute values](http://mathiasbynens.be/notes/unquoted-attribute-values) that can lead to XSS attacks).
- Attribute selectors should only be used where absolutely necessary (e.g., form controls) and should be avoided on custom components for performance and explicitness.
- Series of classes for a component should include a base class (e.g., `.component`) and use the base class as a prefix for modifier and sub-components (e.g., `.component-lg`).
- Avoid inheritance and over nesting—use single, explicit classes whenever possible.
- When feasible, default color palettes should comply with [WCAG color contrast guidelines](http://www.w3.org/TR/WCAG20/#visual-audio-contrast).
- Except in rare cases, don't remove default `:focus` styles (via e.g. `outline: none;`) without providing alternative styles. See [this A11Y Project post](http://a11yproject.com/posts/never-remove-css-outlines/) for more details.

### JS

- No semicolons (in client-side JS)
- 2 spaces (no tabs)
- strict mode
- "Attractive"

### Checking coding style

Run `grunt test` before committing to ensure your changes follow our coding standards.


## License

By contributing your code, you agree to license your contribution under the [MIT license](https://github.com/twbs/bootstrap/blob/master/LICENSE).

Prior to v3.1.0, Bootstrap was released under the Apache License v2.0.