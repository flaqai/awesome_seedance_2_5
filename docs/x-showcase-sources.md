# Seedance 2.5 X video showcase — source notes

[Watch the showcase](../README.md#seedance-25-videos-from-x--watch-inspect-remix) · [Structured source records](x-showcase-sources.json) · [Original prompt library](../prompts/README.md)

Checked on **2026-09-20**. The showcase contains twelve public X posts selected for an explicit Seedance 2.5 claim, an attached video, and a complete prompt in the post body. Each entry links the original post, the original-hosted MP4, and the poster supplied with that media. Model attribution is reported by the account posting the clip; it is not independently authenticated.

## How to use each entry

1. Click the thumbnail or **Watch video** to open the linked MP4. GitHub does not reliably embed arbitrary third-party video players in Markdown, so the preview is a clickable image.
2. Open **Original X post + full author-published prompt** for the complete source wording. A short quotation identifies one useful instruction without mirroring the full post.
3. Expand **Copy the editorial prompt adaptation** for a newly written, compact variant. These variants change scene details and pacing; they have not been tested in this repository and did not produce the linked clips.

The twelve showcase entries are additional reading, separate from the 120 numbered original recipes and the six shared test scenes in each localized prompt file. They are not counted as new translations.

## Latest additions

X07–X12 add performance pacing, craft tutorials, action-lighting continuity, travel storytelling, explicit prop handovers, and place-specific sound design. Selection favors a useful prompting technique and a recoverable full source prompt, not popularity or an unverified quality ranking. X07's post credits @techhalla for its prompt idea; the posting account is preserved separately. X08's storyboard timing and X09's requested 4K aesthetic differ from uploaded metadata and are explicitly noted.

## Verification and limitations

Direct X page retrieval returned HTTP 403 during research. Public post text and media metadata were retrieved through [FxTwitter's API](https://github.com/FixTweet/FxTwitter), with exact account/status IDs preserved. All twelve MP4 URLs returned HTTP 200 with `video/mp4`; all twelve thumbnails returned HTTP 200 with `image/jpeg`. These are availability and provenance checks, not playback, quality scoring, or independent reproduction tests. The [JSON records](x-showcase-sources.json) preserve source IDs, dates, media URLs, dimensions, durations, and verification status.

Several posts request portrait or 4:3 generation, while their uploaded media is landscape. The showcase lists both values rather than treating upload dimensions as evidence of the generation settings. Files may have been resized, padded, edited, or re-encoded; the metadata does not establish which occurred.

The discovery process used [ZeroLu/awesome-seedance](https://github.com/ZeroLu/awesome-seedance) for its video/source/prompt presentation pattern and a [Seedance 2.5 community gallery](https://cheerselfai.com/en/demo/seedance-2-5) to locate candidate status links. Entries were then checked against their own post data. The ZeroLu collection labels itself Seedance 2.0; those videos were not relabeled as 2.5. Posts that only said “prompt in replies,” without a recovered prompt, were excluded from this selection.

## Credits and maintenance

The linked videos, thumbnails, and quotations remain third-party material and are excluded from this repository's MIT license. The listed account is the posting source, not a claim that we verified sole authorship. No third-party video files have been copied into the repository.

If a media URL stops working, use the original X link; if the source is deleted or no longer supports the model/prompt claim, remove or clearly mark the entry. To propose another example, open an issue with its X status URL, video link, model evidence, and the exact location of its prompt. Authors may also request attribution corrections or removal.
