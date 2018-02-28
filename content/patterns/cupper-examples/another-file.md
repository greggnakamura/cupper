+++
title = "Examples"
tags = ["example tag", "another tag"]
+++

You can just write **markdown** here. But don't forget there are lots of shortcodes to help you with writing and showing off code too. See [the documentation for **Cupper**](https://thepaciellogroup.github.io/cupper/) for full details.

I can reference the {{% pattern "My Second Pattern File" %}} pattern here.

---

{{% note %}}
Here's an example of a note shortcode for adding little "oh and also" notes to your patterns' documentation.
{{% /note %}}

---

{{% warning %}}
This is a warning! It's about something the reader should be careful to do or to avoid doing. Use warnings when something could go wrong.
{{% /warning %}}

{{% expandable label="A section of dummy text" level="2" %}}
Here is some markdown including [a link](https://twitter.com/heydonworks). Donec erat est, feugiat a est sed, aliquet pharetra ipsum. Vivamus in arcu leo. Praesent feugiat, purus a molestie ultrices, libero massa iaculis ante, sit amet accumsan leo eros vel ligula.
{{% /expandable %}}

## WCAG Refences
{{% wcag include="1.2.1, 1.3.1, 4.1.2" %}}

### Full Descriptions
{{% wcag include="1.3.1, 4.1.2" descriptions="true" %}}

---

## Visually hidden snippet
{{% snippet file="visually-hidden.md" %}}

---

## Table of Content

Can be disabled with front matter setting.
```md
+++
title = "My page with a few headings"
toc = false
+++
```

---

{{<youtube w7Ft2ymGmfc>}}

---

## Codepen
{{% codePen VpVNKW %}}

---

{{% tested using="Firefox + NVDA, Chrome, Safari iOS + Voiceover, Edge" %}}

---

```html
<button aria-pressed="false">Toggle Me</button>
<style>
  button {
    background: DarkCyan;
    color: white;
    border: 0;
    font-size: 1.5rem;
    padding: 0.5em 1em;
    border-right: 5px solid #000;
    border-bottom: 5px solid #000;
  }

  [aria-pressed="true"] {
    border: 0;
    border-top: 5px solid #000;
    border-left: 5px solid #000;
  }
</style>
<script>
  var toggle = demo.querySelector('[aria-pressed]');

  toggle.addEventListener('click', (e) => {
    let pressed = e.target.getAttribute('aria-pressed') === 'true';
    e.target.setAttribute('aria-pressed', !pressed);
  });
</script>
```

{{<demo>}}
<button aria-pressed="false">Toggle Me</button>
<style>
button {
  background: DarkCyan;
  color: white;
  border: 0;
  font-size: 1.5rem;
  padding: 0.5em 1em;
  border-right: 5px solid #000;
  border-bottom: 5px solid #000;
}

[aria-pressed="true"] {
  border: 0;
  border-top: 5px solid #000;
  border-left: 5px solid #000;
}
</style>
<script>
var toggle = demo.querySelector('[aria-pressed]');

toggle.addEventListener('click', (e) => {
  let pressed = e.target.getAttribute('aria-pressed') === 'true';
  e.target.setAttribute('aria-pressed', !pressed);
});
</script>
{{</demo>}}