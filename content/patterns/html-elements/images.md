+++
title = "Images"
tags = ["html elements"]
+++

{{% note %}}
**If you were to disable images from loading on your website, would it still convey the same meaning?**
{{% /note %}}

---

Images are a valuable source of information. As the saying goes, *"a picture is worth a thousand words"*. When coupled with content, images provide a way of conveying meaning through the use of visuals. **However, sometimes people are not able to see these images.** A few scenarios are:

- a person with a vision disability (*color blindness, low-vision, complete blindness*)
- a person who has disabled loading of images to save data
- a person on a slow network, causing image loading issues
- search engines

## Alternate Text
In order to describe images, the `<img>` element has an `alt` attribute whose value is used to make visual information accessible. Alternate text allows information to be rendered in a variety of ways (i.e. - screen reader).

```html
<img src="/path/to/image" alt="Image description" />
```

### Usage Guidelines

**All images must have an `alt` attribute.**

- Images are invisible to screen readers if `alt` attribute is not provided.
- Screen readers will skip any image without an `alt` attribute

**Not all `alt` attributes require a value.**

- In cases where an image is purely decorative, the `alt` attribute can be left empty.
- Screen readers will skip any image with an empty `alt` value.

### Alternate Text Decision Tree

Providing appropriate alternate text can be a difficult. To facilitate this process, below are a few resources that can be used as a reference:

- <a href="https://www.w3.org/WAI/tutorials/images/decision-tree/" target="_blank">An alt Decision Tree<span class="vh">, opens in a new tab, window</span></a>
- <a href="http://myaccessible.website/Infographic/Images/making-images-accessible-alt-text" target="_blank">Infographic: Making Images Accessible<span class="vh">, opens in a new tab, window</span></a>

---

## WCAG Refences
{{% wcag include="1.1.1" descriptions="true" %}}