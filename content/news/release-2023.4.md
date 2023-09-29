---
title: "Release 2023.4"
date: 2023-09-28T23:25:21+02:00
---

We're pleased to announce a [new release of the Nope Foundry project][release].
It's been only a month since the launch, but we already have a number of new
features we would like to show off.

The key feature of this release is probably the addition of the **fractal
noise**, the corner stone of any serious CGI work.

{{< video gaVoxfoy2CY >}}

By default the noise is in greyscale, but it comes with a **color remapping
filter** which can be used to build any arbitrary gradient pattern to apply on
a source. Since it's a generic rendering filter, it is of course not limited to
the noise.

![Colormap filter](/img/news/2023.4/colormap.png#centered)

Another thing we wanted to do for a very long time was to make it easy to
**create a texture from any given part of the graph**. We already had the
`RenderToTexture` node, but we needed something simpler to use. We decided to
make it possible for the `Texture2D` node to directly accept another tree of
nodes as data source. This makes it extremely simple to build masks, create
displacement map, or apply any post-processing of your imagination, on any given
part of the graph.

More low-key but still impactful for creators, the `Eval*` nodes gained the
ability to pick from **multidimensional inputs**. This is particularly useful
for example when you want to work with vector based live control inputs such
as colors.

![Eval color](/img/news/2023.4/evalcolor.png#centered)

More specific but still useful for presentation, comparison and experiments, a
`GridLayout` node was added to display a number of subscenes following an
**arbitrary grid layout**.

{{< video T6dxX47-xFU >}}

The **viewer** also received a lot of fixes, most notably on **Windows**
where we are finally providing a proper **standalone build**. A few other
features also slipped in, such as the **GIF and AV1 export profiles**, and the
possibility to **drag'n drop scripts** directly into the main window.

Finally, we poured a lot of love into the **documentation**. Many pages were
entirely refreshed, and now include (in particular in the howto pages) video
previews with their associated standalone code snippets. They also come with the
visual graph representation to help understanding the graph tree structure.

![Documentation code snippet](/img/news/2023.4/doc-code-snippet.png#centered)

That's it for this release, but as usual for updates and more frequent content
you can follow us on social networks (see the website footer).

[release]: {{< param github >}}/nope.gl/releases/tag/v2023.4
