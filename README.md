<div align="center">
  <img src="./banner.svg" alt="docs.ubports.com banner" width="100%" />

  <h1>docs.ubports.com</h1>
  <p><strong>Документация UBports в едином рабочем репозитории.</strong> Исходники сайта, сборка, переводы и документационный workflow.</p>

  <p>
    <img src="https://img.shields.io/badge/Documentation-UBports-111827?style=for-the-badge&logo=readthedocs&logoColor=22C55E" alt="Documentation UBports" />
    <img src="https://img.shields.io/badge/Python-Sphinx-111827?style=for-the-badge&logo=python&logoColor=22C55E" alt="Python Sphinx" />
    <img src="https://img.shields.io/badge/translations-po%20files-111827?style=for-the-badge&logoColor=22C55E" alt="Translations" />
    <img src="https://img.shields.io/badge/site-docs.ubports.com-22C55E?style=for-the-badge&labelColor=0B1220" alt="Site" />
  </p>
</div>

```text
> repo: docs.ubports.com
> pipeline: build docs / update translations / publish site
> role: source of truth for UBports documentation
```

## обзор

Этот репозиторий нужен для сборки и сопровождения сайта документации `UBports`, включая локальную сборку, обновление переводов и документированный процесс внесения изменений.

### Как вносить изменения

Правила и рекомендации по участию описаны здесь:
- https://docs.ubports.com/en/latest/contribute/documentation.html

Перед отправкой изменений лучше придерживаться всех требований с этой страницы, иначе вклад могут не принять.

### Сборка документации

Собрать документацию можно командой из корня репозитория:

```bash
./build.sh
```

Скрипт также создаст виртуальное окружение в `~/ubportsdocsenv`, если его еще нет.

После завершения сборки открыть результат можно локально, например так:

```bash
firefox _build/html/index.html
```

### Обновление переводов

Чтобы обновить `.po`-файлы переводов, выполните:

```bash
./update-translations.sh
```

Чтобы добавить новый язык, внесите его ISO-код в `languagues.sh`, а затем снова запустите:

```bash
./update-translations.sh
```

## контакты

<p>
  <a href="https://github.com/GradusXaker"><img src="https://img.shields.io/badge/GitHub-GradusXaker-111827?style=flat-square&logo=github&logoColor=22C55E" alt="GitHub" /></a>
  <a href="https://vk.com/gradus_xaker"><img src="https://img.shields.io/badge/VK-gradus__xaker-111827?style=flat-square&logo=vk&logoColor=22C55E" alt="VK" /></a>
  <a href="mailto:gradus_xaker@mail.ru"><img src="https://img.shields.io/badge/email-write-111827?style=flat-square&logo=gmail&logoColor=22C55E" alt="Email" /></a>
</p>

