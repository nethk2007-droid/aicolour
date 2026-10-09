# GRADE — Natural Colour Studio

A Next.js MVP for natural, non-generative photo colour grading.

## What works
- Upload JPG, PNG, and WebP photos (up to 25 MB).
- Client-side preview using Canvas pixel adjustments.
- Lightweight image-statistics-based natural-grade suggestions.
- Manual exposure, contrast, highlights, shadows, temperature, tint, saturation, and vibrance controls.
- Processing timeline, edit history, original toggle, and PNG export.
- Photo processing runs in the browser; images are not sent to a server.

## Important limitations
This is a functional MVP, not a trained AI colour-grading model. Its automatic suggestions use simple image statistics and heuristics. It does not perform semantic scene understanding or reliable skin segmentation. The comparison slider UI is currently a visual control only; use **Show original** to toggle the original image. Preview and export use equivalent pixel operations, but future production work should unify the rendering function to guarantee exact parity.

## Run locally
Requires Node.js 20.9+.

```bash
npm install
npm run dev
```

Open http://localhost:3000.

## Deploy to Vercel
1. Create a new Git repository and upload these project files.
2. Import the repository into Vercel.
3. Keep the framework preset as Next.js.
4. Use the default build command (`npm run build`) and output settings.
5. Click Deploy.

No environment variables or API keys are required for this MVP.
