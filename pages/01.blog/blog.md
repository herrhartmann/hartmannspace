---
title: Blog
hide_git_sync_repo_link: false
sitemap:
    changefreq: monthly
body_classes: 'header-dark header-transparent'
hero_classes: 'text-light title-h1h2 overlay-dark-gradient hero-medium parallax'
blog_url: /blog
show_sidebar: true
show_breadcrumbs: true
show_pagination: true
modular_content:
    items: '@self.modular'
    order:
        by: folder
        dir: dsc
content:
    items:
        - '@self.children'
    limit: 6
    order:
        by: date
        dir: desc
    pagination: true
    url_taxonomy_filters: true
bricklayer_layout: true
display_post_summary:
    enabled: false
feed:
    limit: 10
    description: 'Sample Blog Description'
pagination: true
child_type: item
media_order: 'mountains_blog.jpg,giammarco-boscaro-zeH-ljawHtg-unsplash.jpg'
hero_image: giammarco-boscaro-zeH-ljawHtg-unsplash.jpg
menu: Material
---

[center][ui-animated-text words="Deutsch, Englisch" animation="push" element="h2"]Materialien:[/ui-animated-text]
[/center]