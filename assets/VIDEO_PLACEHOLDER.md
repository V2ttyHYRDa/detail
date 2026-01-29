# Hero Showcase Video Placeholder

This is a placeholder for `hero-showcase.mp4`.

## Video Specifications:
- **Dimensions:** 1080×1350px (portrait 4:5 aspect ratio)
- **Duration:** 10-30 seconds (will loop automatically)
- **Format:** MP4 (H.264 codec)
- **Target Size:** 2-5MB
- **Frame Rate:** 30fps recommended
- **Audio:** None (muted video)

## Content Suggestions:
1. Ceramic coating application process
2. Car transformation before/after
3. Close-up shots of glossy finishes
4. Detailing work in progress
5. Reflections and shine demonstrations

## How to Replace This Placeholder:
1. Export your video as MP4 (H.264)
2. Optimize using HandBrake or similar tool
3. Name it `hero-showcase.mp4`
4. Replace this file in the `/assets/` folder
5. Delete this `VIDEO_PLACEHOLDER.md` file

## Quick Video Optimization with FFmpeg:
```bash
ffmpeg -i your-video.mov -vf "scale=1080:1350:force_original_aspect_ratio=decrease" -c:v libx264 -preset slow -crf 28 -an hero-showcase.mp4
```

This command will:
- Scale video to 1080×1350
- Use H.264 codec
- Optimize for web (CRF 28 = good quality/size balance)
- Remove audio track
- Output as hero-showcase.mp4
