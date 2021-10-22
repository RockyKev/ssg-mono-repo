# SSG Mono Repo

A test of various Javascript-based SSG tools.

## sveltekit

1. install sveltekit - https://kit.svelte.dev/docs#introduction-getting-started
2. install a adapter - https://kit.svelte.dev/docs#configuration-adapter
    https://github.com/sveltejs/kit/tree/master/packages/adapter-static

3. install the add-on - https://github.com/svelte-add/mdsvex

Pros:
Pretty straightforward. got it working right out of the box. 
Really clean way to import dynamic components if I want it. 
Really slick.
Installing mdsvex was so slick. It added the code I need automagically. 
Super fast since it uses VITE.

Things to be aware of:
* It'snot using `.md`, but `.svx`. 
* I had to build my own blog page. 
* It's still in a prototype phase. It says it everywhere
* I had to 



## nextjs (NextJS)

1. npx create-next-app nextjs-blog --use-npm --example "https://github.com/vercel/next-learn/tree/master/basics/learn-starter"

2. install the official plugin: https://mdxjs.com/getting-started/next/
    - added a next.config.js

PROS:
Works right out of the box.

Things to be aware of: 
* It took a while to install, and takes a while to build. (Since it's using webpack)
* MDX just generates the markdown, including the frontmatter. So I needed to build my own wrapper to get this working.



## Vue / Nuxt 

## elventy

## hexo
