# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Primary users are adults supporting young children's speech, language, and early literacy — parents, teachers, caregivers, and speech/occupational therapists. They come to buy or share the book, download free activities, and find developmental resources. Children enjoy the activities; adults are the decision-makers.

## Product Purpose

Companion website for the picture book *Rusty the Raccoon is Scared of the Dark* by Michelle Trotta. Success means visitors can purchase the book, access free printables and literacy resources, meet the author, and engage with supporting media (including ASL) — all in service of friendship, courage, acceptance, and speech/language development.

## Positioning

Unlike a generic children's-book storefront, this site is built around a book written by a practicing speech-language pathologist and mother. The story is intended as a developmental tool, and the site backs that claim with free printable activities and curated speech/literacy resources for home, classroom, and therapy use.

## Operating Context

Visitors browse a small static marketing site: home (purchase CTA), about/story and mission, author bio, downloadable activity PDFs, external SLP/literacy resource links, embedded videos (Kickstarter, ASL storytelling, read-aloud), and email contact. Social follow happens via Facebook, Instagram, and YouTube. The book is sold on Amazon; Fresh Beginnings Publishing is the publisher.

## Capabilities and Constraints

- Static Astro site deployed to Netlify (`rustytheraccoon.com`); original Wix site retired.
- Pages: Home, About, Author, Activities, Resources, Videos, Contact, 404.
- Free downloadable activity PDFs (11) hosted under `public/activities/`.
- Amazon purchase link is the primary commercial CTA.
- Contact is email-only (`Freshbeginningspublishing@gmail.com`); no on-site form backend required today.
- Content and structure should stay faithful to the archived original site in `scrape/` unless explicitly changed.
- Undecided: timing and marketing treatment for future books in the overcoming-fears animal series.

## Brand Commitments

- Product/book name: *Rusty the Raccoon is Scared of the Dark*; site brand often shortens to "Rusty the Raccoon."
- Author: Michelle Trotta (Ohio-based speech-language pathologist and mother); byline appears in the header.
- Illustrator: Alisha Uguccini.
- Publisher: Fresh Beginnings Publishing.
- Characters and motifs: Rusty the raccoon, Squeaks the squirrel, firefly jar / firefly-glow signature.
- Voice: warm, encouraging, accessible to parents and professionals; child-friendly without talking down to adults.
- Binding assets: book cover art, character illustrations, raccoon logo, author headshot, activity artwork — do not invent substitute brand art.

## Evidence on Hand

- Book cover and character illustrations in `src/assets/images/` (from the Alisha Uguccini / Fresh Beginnings materials).
- Author headshot and bio copy on `/author`.
- Eleven activity PDFs in `public/activities/`.
- Twelve curated external resource links on `/resources`.
- Three YouTube embeds on `/videos` (Kickstarter, ASL by Hannah Bissonette, full read-aloud).
- Live Amazon paperback listing and social profiles (Facebook, Instagram, YouTube).
- Full original-site scrape and content manifest in `scrape/` (reference only; not part of the build).
- Do not fabricate testimonials, sales figures, awards, press quotes, or additional books/series titles beyond what is already published on the site.

## Product Principles

1. Serve the adult helper first — make buy, download, and learn paths obvious without burying them in decoration.
2. Keep the book and its artwork as the authority; the site supports the story, it does not reinvent it.
3. Free resources are part of the product promise, not a secondary promo.
4. Stay faithful to confirmed copy, credits, and links; invent nothing that looks like proof.
5. Remain usable for parents at home and professionals in classroom or therapy settings.

## Accessibility & Inclusion

English-language site with skip-to-main link and semantic page structure already present. An ASL storytelling video is a confirmed inclusion asset. No formal WCAG target or additional assistive requirements have been established yet — treat clear hierarchy, readable type, and keyboard-friendly navigation as the baseline until specified.
