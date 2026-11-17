# IskraJoDesign портфолио

Еден `index.html` и папка `img/` со сите слики (90). Нема build, нема зависности. Сајтот работи на македонски (стандарден), англиски и српски (кирилица), без освежување на страницата.

## Објавување на GitHub Pages

1. Качи ги `index.html` и целата папка `img/` во коренот на репото (Add file → Upload files).
2. Settings → Pages → Source: "Deploy from a branch", Branch: `main`, папка `/ (root)` → Save.
3. По 1 до 2 минути сајтот е онлајн.

Важно: `og:url`, `og:image` и `canonical` во `index.html` покажуваат на `https://iskrajodesign.github.io/iskrajodesign/`. Ако сајтот го ставиш во друго репо, замени ја таа адреса на 4 места во `<head>`.

## Што уште треба да се дополни

- Искуства: трите картички се празни места.
- „Логистика и складирање“: има слика и линк, а статусот и краткиот опис чекаат твој текст (во `var D`, клуч `logi`, полиња `st` и `l`).
- FitTrack и Рибен ресторан немаат линк, па копчето „Целиот сајт во живо“ не се прикажува.
- Иконата за Инстаграм е без линк. Иконата за телефон води до Calendly.
- Формуларот праќа преку FormSubmit на iskrajodesign@gmail.com. Првиот пат FormSubmit праќа е-маил за потврда.

## Адреса (ПОСТАВИ ПРЕД ОБЈАВУВАЊЕ)

Старата адреса iskrajodesign.github.io/iskrajodesign/ НЕ се користи. Сите места што зависат од новата GitHub Pages адреса го носат привремениот текст `https://POSTAVI-NOVA-ADRESA/`: canonical, og:url, og:image и JSON-LD во index.html, sitemap.xml и robots.txt. Кога адресата е потврдена, пуштете од папката portfolio-export:

    python3 postavi-adresa.py https://ВАШАТА-НОВА-АДРЕСА/ iskrajodesign-portfolio

## Фонтови

Фонтовите (Old Standard TT 400, Spectral 400, JetBrains Mono 400, Unbounded 500 и 800, латиница и кирилица) се вградени директно во index.html, па нема папка fonts и нема повици кон Google. Вкупно 94 датотеки, што влегува во едно качување на GitHub (лимит 100). Фонтовите се Fontsource, лиценца OFL.

## Корекции v63 до v65

- `<main>` и skip линк, најмал текст 12px, focus прстен, loading состојба на формуларот, width и height на сликите.
- Менито: „Проекти“ води до „Останати проекти“. Футер: само две икони (Instagram и LinkedIn), без линкови.
- Hover на CTA копчињата со обратни бои.
- Редоследот: „Услуги“ е пред „Зошто јас“.
