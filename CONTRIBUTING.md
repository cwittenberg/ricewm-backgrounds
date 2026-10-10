# Contribute a public-domain wallpaper

1. Add a PNG, JPEG or WebP under `submissions/your-slug/`. Use a genuine
   landscape image at least 1600×900, no animation, no added logos, no identifiable
   private people, at most 24 MiB and 24 megapixels. Prefer 3840×2160 or larger
   within these bounds. Keep your submitted source; the operator generates WebP.
2. Add `wallpaper.json` beside it using the example below. Provide the original
   creator, a direct source record and verifiable evidence of public-domain status.
   Include 1–12 distinct lowercase tags (maximum 32 characters each) describing
   the style, subject, colours or palette, such as `modern`, `minimal`, `dark`,
   `neon`, `space`, `anime`, `catppuccin` or `gruvbox`. Use palette names only
   when the artwork actually matches that palette. Tags are reviewed and used
   by the app’s tag filter.
   Museum CC0 records and an explicit CC0 dedication by the actual creator are
   suitable evidence. A generic website footer, repository license, stock-site
   download button or assertion without evidence is insufficient.
3. Submit a PR and complete its certification. Do not change generated
   `wallpapers/`, `catalog/`, policies or workflows as part of an image submission.
4. RiceWM.org vets the bytes and checks your evidence. The operator must approve
   the exact converted image before inclusion in the public app. Changes restart
   review. We may ask for better evidence or decline unsuitable submissions.

By submitting, you certify that the wallpaper is genuine and is public domain
worldwide, or that you own all necessary rights and dedicate them under CC0 1.0.
To the extent you hold rights in the wallpaper, submission, metadata or derivative,
you apply the [CC0 1.0 Universal dedication and fallback license](https://creativecommons.org/publicdomain/zero/1.0/).
You waive and agree not to assert rights you can legally waive, and request no
copyright payment, restriction or exclusive license. You certify that no third
party's copyright or other rights prevent anyone from using, adapting or
redistributing the image. You cannot waive another person's rights; where a right
cannot legally be waived, CC0's terms govern. False certification is grounds for
removal and contributor exclusion. Submission does not guarantee acceptance.

Do not send personal contact or copyright complaints through a public PR.
Use the [private reporting form](https://account.env.now/wallpaper-copyright).

```json
{
  "id": "wp-your-slug",
  "name": "Mountain dawn",
  "author": "Original creator",
  "category": "landscape",
  "tags": ["landscape", "minimal", "dark"],
  "input": "submissions/your-slug/source.jpg",
  "source": "https://example.org/original-source-record",
  "rights": {
    "license": "CC0-1.0",
    "evidence": "https://example.org/individual-cc0-evidence",
    "basis": "Explain who owns the rights and where they applied CC0, or establish worldwide public-domain status.",
    "attestationVersion": "ricewm-public-domain-1",
    "certifiedPublicDomain": true,
    "noThirdPartyRights": true,
    "waiveOwnedRights": true
  }
}
```

For independently established worldwide public-domain works, use `Public-Domain`
and document the basis and any separate rights in the photograph or scan. Avoid
country-only public-domain claims when the image remains protected elsewhere.
