---
title: Preparing Content for Translation
seo-title: Preparing Content for Translation
description: Learn how to prepare content for translation.
seo-description: Learn how to prepare content for translation.
uuid: 369630a8-2ed7-48db-973e-bd8213231d49
contentOwner: Guillaume Carlino
products: SG_EXPERIENCEMANAGER/6.4/SITES
topic-tags: site-features
content-type: reference
discoiquuid: 8bd67d71-bcb7-4ca0-9751-3ff3ee054011
feature: Language Copy
exl-id: 1a7fe230-093b-4d2b-95cb-f9479c0febe5
---
# Preparing Content for Translation{#preparing-content-for-translation}

Multilingual web sites generally provide some amount of content in multiple languages. The site is authored in one language and then translated into other languages. Generally, multilingual sites consists of branches of pages, where each branch contains the pages of the site in a different language.

The sample Geometrixx Demo Site includes several language branches and uses the following structure:

```xml
/content
    |- geometrixx
             |- en
             |- fr
             |- de
             |- es
             |- it
             |- ja
             |- zh
```

Each language branch of a site is called a language copy. The root page of a language copy, known as the language root, identifies the language of the content in the language copy. For example, `/content/geometrixx/fr` is the language root for the French language copy. Language copies must use a [correctly-configured language root](/help/sites-administering/tc-prep.md#creating-a-language-root) so that the correct language is targeted when translations of a source site are performed.

The language copy for which you originally author site content is the language master. The language master is the source that is translated into other languages.

Use the following steps to prepare your site for translation:

1. Create the language root of your language master. For example, the language root of the English Geometrixx demo site is /content/geometrixx/en. Ensure that the language root is correctly configured according to the information in [Creating a Language Root](/help/sites-administering/tc-prep.md#creating-a-language-root).
1. Author the content of your language master. 
1. Create the language root of each language copy for your site. For example, the French language copy of the Geometrixx sample site is /content/geometrixx/fr.

After you prepare your content for translation, you can automatically create missing pages in your language copies and associated translation projects. (See [Creating a Translation Project](/help/sites-administering/tc-manage.md).) For an overview of the content translation process in AEM, see [Translating Content for Multilingual Websites](/help/sites-administering/translation.md).  

## Creating a Language Root {#creating-a-language-root}

Create a language root as the root page of a language copy that identifies the language of the content. After you create the language root, you can create translation projects that include the language copy.

To create the language root you create a page and use an ISO language code as the value for the Name property. The language code must be in one of the following formats:

* `<language-code>`The supported language code is a two-letter code as defined by ISO-639-1, for example `en`.

* `<language-code>_<country-code>` or `<language-code>-<country-code>`The supported country code is a lower-case or upper-case two-letter code as defined by ISO 3166, for example `en_US`, `en_us`, `en_GB`, `en-gb`.

You can use either format, according to the structure that you have chosen for your global site.  For example, the root page of the French language copy of the Geometrixx site has `fr` as the Name property. Note that the Name property is used as the name of the page node in the repository, and therefore determines the path of the page. (http://localhost:4502/content/geometrixx/fr.html)

The following procedure uses the touch-optimized UI to create a language copy of a web site. For instructions that use the Classic UI, see [Creating a Language Root Using the Classic UI](/help/sites-administering/tc-lroot-classic.md).

1. Navigate to Sites.
1. Click or tap the site for which you want to create a language copy.

   For example, to create a language copy of the Geometrixx Outdoors site, you would click or tap Geometrixx Outdoors Site. 

1. Click or tap Create, and then click or tap Create Page.

   ![chlimage_1-21](assets/chlimage_1-21.png)

1. Select the page template and then click or tap Next.
1. In the Name field type the country code in the format of `<language-code>` or `<language-code>_<country-code>`, for example `en`, `en_US`, `en_us`, `en_GB`, `en_gb`. Type a title for the page.

   ![chlimage_1-22](assets/chlimage_1-22.png)

1. Click or tap Create. In the confirmation dialog box, click or tap either **Done** to return to the Sites console, or **Open** to open the language copy.

## Seeing the Status of Language Roots {#seeing-the-status-of-language-roots}

The touch-optimized UI provides a References panel that shows a list of language roots that have been created.

![chlimage_1-23](assets/chlimage_1-23.png)

The following procedure uses the touch-optimized UI to open the References panel for a page.

1. On the Sites console, select a page of the site and then click or tap **References**.

   ![chlimage_1-24](assets/chlimage_1-24.png)

1. In the references panel, click or tap **Language Copies**. The Language Copies panel shows the language copies of the web site.
