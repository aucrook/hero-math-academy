# Hero Math Academy

A gamified, superhero-themed math adventure for 2nd graders. Original characters only (no Marvel/DC).

## Play locally

Open `index.html` in a browser, or from this folder:

```bash
python3 -m http.server 8080
```

Then visit http://localhost:8080

## Publish (GitHub Pages — recommended)

Needs a one-time GitHub login on this machine:

```bash
gh auth login
cd /workspace/hero-math
gh repo create hero-math-academy --public --source=. --remote=origin --push
gh api repos/$(gh api user -q .login)/hero-math-academy/pages -X POST -f build_type=legacy -f source.branch=main -f source.path=/
```

Live URL will be: `https://<your-github-username>.github.io/hero-math-academy/`

### Alternatives

- **Netlify**: `npx netlify-cli login` then `npx netlify-cli deploy --dir=. --prod`
- **Vercel**: `npx vercel login` then `npx vercel --prod`

Anonymous Netlify deploys expire in ~1 hour unless claimed — not suitable as the permanent link.

## Skills covered (Grade 2)

Addition within 20 · Add/subtract within 100 · Place value · Skip counting · Comparing · Time to 5 minutes · Coin money · Word problems · Arrays / intro multiplication · Final mixed boss battle
