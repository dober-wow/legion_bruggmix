<!-- md2html-theme: emerald-nightmare -->
s
# Auto Theme Demo

This page demonstrates the per-document theme metadata that `md2html` now understands.
s
- A theme hint is supplied through the HTML comment at the very top of the file.
- When you run the converter with `--theme auto`, the output for this document will use the **emerald-nightmare** palette.
- Other documents can choose their own themes without passing new CLI flags.

> Tip: you can also express the theme inside front matter:
>
> ```markdown
> ---
> md2html:
>   theme: trial-of-valor
> ---
> ```

## Next Steps

1. Regenerate the site with:
   ```bash
   md2html convert legion_bruggmix --output docs --theme auto --recursive
   ```
2. Commit the generated HTML together with this markdown sample.
3. Push to main and confirm the deployment. The new page will surface at `docs/demo-theme-auto.html`.
