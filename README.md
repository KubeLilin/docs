
## 1. Install dependencies

```bash
npm install
```
You can skip when Press Ctrl + C to stop install hugo.
## 2. Instal hugo
Mac
```bash
brew install hugo
```
or other os:
```bash
go install -tags extended github.com/gohugoio/hugo@latest

hugo version
```

## 3. Start Hugo’s development server to view the site.
```bash
hugo server
```
Press Ctrl + C to stop Hugo’s development server.

## Add content 
Add a new page to your site.
```bash
hugo new posts/my-first-post.md
```
Hugo created the file in the content/posts directory. Open the file with your editor.
```markdown
---
title: "My First Post"
date: 2022-11-20T09:03:20-08:00
draft: true
---
```
Notice the draft value in the front matter is true. By default, Hugo does not publish draft content when you build the site. Learn more about draft, future, and expired content.

Add some markdown to the body of the post, but do not change the draft value.
```markdown
---
title: "My First Post"
date: 2022-11-20T09:03:20-08:00
draft: true
---
## Introduction

This is **bold** text, and this is *emphasized* text.

Visit the [Hugo](https://gohugo.io) website!
```
Save the file, then start Hugo’s development server to view the site. You can run either of the following commands to include draft content.

```bash
hugo server --buildDrafts
hugo server -D
```
View your site at the URL displayed in your terminal. Keep the development server running as you continue to add and change content.


