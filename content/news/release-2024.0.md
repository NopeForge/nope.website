---
title: "Release 2024.0"
date: 2024-02-02T19:33:09+01:00
---

Our [first release for 2024][release] just landed.

The main feature of this release is probably the introduction of the **blur
nodes**. The `FastGaussianBlur` in particular allows blurring textures in real
time (even on mobile devices). Its resolution independent blurriness parameter
makes it suitable for creating content agnostic effects.

{{< video 9cKyBFGbXcw >}}

We're currently preparing the foundation for various masking features. The
first one we're introducing in this release is the `Selector` filter. This
filter makes it easy to **create a mask by selecting colors** according to their
lightness, chroma or hue. In the following demo, we're cycling through the hue
wheel to select the different colors of an [artwork by muju][muju-mute-5], and
blending the resulting selection onto a greyscale version of that same picture.

{{< video 33ZOXXcgbu4 >}}

So far the Nope releases were only distributing a scene viewer, but a few more
tools were actively developed behind the scene, and available in the development
environment. We've decided to add one of them to the release: **the diff
tool**, a simple tool to compare videos (and images):

{{< video hjOH6nHdw6o >}}

In addition to the usual batch of bug fixes, various **important changes were
made to the API** as we're laying down the core foundations for an incoming
redesign. For details, you can refer to the [changelog].

Now, an important change not directly related to the software itself is that
the **Nope Forge company has been created** to back up the project financially.
This means that we now [accept donations][contribute], and we're also open
to consulting work. We hope this will make the project sustainable in the long
term. Our mission doesn't change, and the project remains free and open-source.

[release]: {{< param github >}}/nope.gl/releases/tag/v2024.0
[muju-mute-5]: https://www.deviantart.com/muju/art/Mute-5-0-347320002
[changelog]: {{< param github >}}/nope.gl/blob/v2024.0/CHANGELOG.md
[contribute]: {{< ref "/contribute" >}}
