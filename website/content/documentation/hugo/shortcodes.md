---
title: "Shortcodes"
weight: 50
sidenav:
  toc:
    includehtml: true
---
This theme provides the following Hugo shortcodes.

## `callout` Shortcode

Creates a callout block.

- `class` (*optional*): Additional CSS class(es) (space-separated) to apply to
  the callout.

## `imagemap` Shortcode

### `area` Shortcode

## `usa-alert` Shortcode

An alert keeps users informed of important and sometimes time-sensitive changes.

The `usa-alert` shortcode supports these parameters:

- `type` (*optional*, default: `info`): The type of alert, must be one of `info`,
  `error`, `warning`, or `success`
- `heading` (**required**): The text to display in the alert heading
- `class` (*optional*): Additional CSS class(es) (space-separated) to apply to
  the alert
- `bodyClass` (*optional*): Additional CSS class(es) (space-separated) to apply
  to the alert body paragraphs

The inner content within the `usa-alert` shortcode will be used as the body content
within the the Alert.

## `usa-graphic-list` Shortcode

The graphic list is used to showcase a number of related items and their respective
images in a grid pattern.

This should likely contain multiple `usa-media-block` shortcodes to define the content.

### `usa-media-block` Shortcode

The `usa-media-block` shortcode supports these parameters:

- `image` (**required**): the URL to the image to use for the block
- `imageAlt` (**requied**): the alt text to use for the image
- `title` (**required**): the heading text for the block

The inner content of the `usa-media-block` shortcode will be used as the text
beside the provided image within the block.

## `usa-grid-container` Shortcode

Creates a `usa-grid-container` element for arranging content two-dimensionally.

The `usa-grid-container` shortcode supports these parameters:

- `class` (*optional*): Additional CSS class(es) (space-separated) to apply to
  the container

The inner content of the `usa-grid-container` shortcode will be used as the
content of the created grid container; usually the direct child elements will
be `usa-grid-row`s which will contain `usa-grid-column`s.

### `usa-grid-row` Shortcode

The `usa-grid-row` shortcode allows creating a grid row; the parent must be a
`usa-grid-container` (an error will be thrown if this is not the case).

The `usa-grid-row` shortcode supports these parameters:

- `class` (*optional*): Additional CSS class(es) (space-separated) to apply to
  the row

The inner content of the `usa-grid-row` shortcode will be used as the content of
the created grid row; usually the direct child elements will be `usa-grid-column`s.

### `usa-grid-column` Shortcode

The `usa-grid-column` shortcode allows creating columns in a `usa-grid-row` within
a `usa-grid-container`.

The `usa-grid-row` shortcode supports these parameters:

- `class` (*optional*): Additional CSS class(es) (space-separated) to apply to
  the row

The inner content of the `usa-grid-column` shortcode will be used directly as the
content of the created column element on the page.

## `usa-hero` Shortcode

Heroes are used at the top of your landing page to help set the tone for the content
of your site and to help users understand what your brand is all about. The hero
offers a callout which provides a high-level overview of the content on the site
and will often reference the hero image that sits behind it.

The `usa-hero` shortcode supports these parameters:

- `image` (*optional*, default: no image): the URL to the image to use for the
  background of the hero
- `calloutText` (**required**): the text to use in the callout in the hero
- `calloutAltText` (*optional*): additional text to use in the callout header after
  the main text
- `buttonText` (**required**): the text to use on the call to action button
- `buttonURL` (**required**): the URL to navigate to when the button is clicked

The inner content within the `usa-hero` will be used as paragraph text within
the callout.

## `usa-intro` Shortcode

Displays a `usa-intro` class `<p>`.

The `usa-intro` shortcode supports these parameters:

- `class` (*optional*): Additional CSS class(es) (space-separated) to apply to
  the `<p>`.

The inner content of the `usa-intro` shortcode will be used as the content of
the `<p>` tag.

## `usa-section` Shortcode

Displays a generic `usa-section` `<section>` element.

The `usa-section` shortcode supports these parameters:

- `id` (*optional*, default: `section-%d`) The HTML `id` attribute to use for
  the `<section>`  
- `class` (*optional*): Additional CSS class(es) (space-separated) to apply to
  the `<section>`.

The inner content of the `usa-section` shortcode will be used within the created
`<section>`.

## `usa-tag` Shortcode

The `usa-tag` shortcode supports these parameters:

- `class` (*optional*): Additional CSS class(es) (space-separated) to apply to
  the Tag.

The inner content of the `usa-tag` shortcode will be used as the text within
the tag.

## `usa-tagline` Shortcode

A wide section of the page to display a tagline, primarily used on the index/landing
page.

The `usa-tagline` shortcode supports these parameters:

- `caption` (**required**): The caption text to display on the left side of the
  tagline.

The inner content of the `usa-tagline` shortcode will be used on the right side
of the tagline.
