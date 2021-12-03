---
# Title, summary, and page position.
linktitle: КНИГА КНИГ
summary: Learn how to use Academic's docs layout for publishing online courses, software documentation, and tutorials.
weight: 1
icon: book-reader
icon_pack: fas

# Page metadata.
title: ОСНОВЫ
date: "2018-09-09T00:00:00Z"
type: book  # Do not modify.
---

## Тайна трех проматерей

Это главное:

* **Алеф** - это нейтральные и биполярные. Те, кто склоняются к 2-ке или 9-ке
* **Шин**  - это 2-ка
* **Мем** - это 9-ка и ее сателит - 4-ка


The `courses` folder may be renamed. For example, we can rename it to `docs` for software/project documentation or `tutorials` for creating an online course.

## Delete courses

**To remove these pages, delete the `courses` folder and see below to delete the associated menu link.**

## Update site menu

After renaming or deleting the `courses` folder, you may wish to update any `[[main]]` menu links to it by editing your menu configuration at `config/_default/menus.toml`.

For example, if you delete this folder, you can remove the following from your menu configuration:

```toml
[[main]]
  name = "Courses"
  url = "courses/"
  weight = 50
```

Or, if you are creating a software documentation site, you can rename the `courses` folder to `docs` and update the associated *Courses* menu configuration to:

```toml
[[main]]
  name = "Docs"
  url = "docs/"
  weight = 50
```

## Update the docs menu

If you use the *docs* layout, note that the name of the menu in the front matter should be in the form `[menu.X]` where `X` is the folder name. Hence, if you rename the `courses/example/` folder, you should also rename the menu definitions in the front matter of files within `courses/example/` from `[menu.example]` to `[menu.<NewFolderName>]`.
