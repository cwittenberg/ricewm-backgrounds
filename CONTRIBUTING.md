# Contribute a wallpaper

Submit polished landscape wallpapers suited to ricing: detailed anime illustrations, cyberpunk streets, cityscapes, space art and atmospheric landscapes. Basic geometric patterns, procedural shapes and simple vector designs are outside this collection's current direction.

1. Add a PNG, JPEG or WebP under `submissions/your-slug/`. Sources must be at least1600×900, landscape, static, at most24MiB and24megapixels. Prefer native4K; do not upscale. Keep the source; the operator generates full WebP and320×180/640×360 previews.
2. Add `wallpaper.json` beside it. Supply the original creator, original source and individual license evidence. Include1–12 distinct lowercase tags, maximum32characters each, describing subject, style or palette. Use `anime`, never `anime-inspired`. Use `catppuccin` only when the actual palette matches it. Label creator-disclosed AI artwork with `ai`; do not invent human-art provenance.
3. Submit a PR and complete all six certifications. Change only your submission files, never generated assets, catalogs, policies or workflows.
4. RiceWM.org checks evidence and converts the image in a restricted container. The operator reviews the exact converted artwork before app inclusion. Changed bytes or rights metadata require a new review. PR code never receives credentials or authority to approve itself.

## Accepted licenses

**CC0 or worldwide public domain:** provide the actual creator's CC0 dedication or an individually documented public-domain record. Certification version `ricewm-public-domain-1` applies. To the extent you own rights in the submission, you dedicate them under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/), including its fallback license, and will not assert incompatible rights, payment or exclusivity. You cannot waive someone else's rights.

**CC BY 3.0 or4.0:** provide an explicit redistribution license from the actual creator covering the individual image. Certification version `ricewm-licensed-1` applies. Supply permanent creator credit, the exact canonical license URL and an accurate description of conversion/cropping changes. The creator retains their rights; you certify authorization to redistribute under that license. Credit travels through the catalog, Quick Wallpapers, the marketplace and saved wallpaper preferences. Downloaded artwork must keep the accompanying attribution information.

A repository license or generic site footer does not establish rights to collected third-party images. Unknown creators, proprietary anime/game fanart without authorization, conflicting redistribution restrictions, CC BY-NC, CC BY-ND and CC BY-SA are not accepted. False certification may cause withdrawal and contributor exclusion. Submission does not guarantee acceptance.

```json
{
  "id": "wp-your-slug",
  "name": "Neon street",
  "author": "Original creator",
  "category": "city",
  "tags": ["city", "cyberpunk", "dark", "neon"],
  "input": "submissions/your-slug/source.jpg",
  "source": "https://example.org/original-image",
  "rights": {
    "license": "CC-BY-4.0",
    "evidence": "https://example.org/individual-license-evidence",
    "basis": "Explain how the actual creator licensed this particular artwork.",
    "attestationVersion": "ricewm-licensed-1",
    "redistributionAuthorized": true,
    "noUnlicensedThirdPartyRights": true,
    "credit": "Neon street — Original creator, original source URL.",
    "licenseUrl": "https://creativecommons.org/licenses/by/4.0/",
    "changes": "Converted to WebP; resized without enlargement; previews cropped to16:9."
  }
}
```

For CC BY3.0, use `CC-BY-3.0` and `https://creativecommons.org/licenses/by/3.0/`. For CC0/public domain, replace the rights object with:

```json
{
  "license": "CC0-1.0",
  "evidence": "https://example.org/individual-cc0-evidence",
  "basis": "Document the actual creator's dedication or worldwide public-domain basis.",
  "attestationVersion": "ricewm-public-domain-1",
  "certifiedPublicDomain": true,
  "noThirdPartyRights": true,
  "waiveOwnedRights": true
}
```

Use `Public-Domain` only with a worldwide basis and separate scan/photograph rights evidence. Send copyright concerns through the [private RiceWM.org reporting form](https://account.env.now/wallpaper-copyright), never personal contact details in a public PR.
